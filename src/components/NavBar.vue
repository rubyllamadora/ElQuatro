<template>
    <div>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#">ElQuatro</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item v-for="(item, index) in menuItems" :to="item.path" :key="index">
          {{ item.name }}
        </b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
        </b-nav-form>

      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
</template>
<script lang="ts">
import Vue from 'vue';
import router from '@/router';
import {
  BNavbar, BNavbarBrand, BNavbarToggle,
  BNavbarNav, BCollapse, BNavItem,
  BNavForm, BFormInput, BButton, BNavItemDropdown, BDropdownItem
  } from 'bootstrap-vue';

export default Vue.extend({
  data() {
    let routes:Array = router.options.routes || [];

    return {
      menuItems: routes || []
    };
  },
  components: {
    'b-navbar': BNavbar,
    'b-navbar-brand': BNavbarBrand,
    'b-navbar-toggle': BNavbarToggle,
    'b-navbar-nav': BNavbarNav,
    'b-collapse': BCollapse,
    'b-nav-item': BNavItem,
    'b-nav-form': BNavForm,
    'b-form-input': BFormInput,
    'b-button': BButton,
    'b-nav-item-dropdown': BNavItemDropdown,
    'b-dropdown-item': BDropdownItem,
  }
});
</script>

