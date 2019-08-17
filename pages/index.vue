<template>
<div>
  <div class="hero is-fullheight has-background">
    <img alt="Hero image" class="hero-background is-transparent" src="@@/assets/img/hero.png" />
    <div class="hero-logo"><img src="@@/assets/img/logo.png" alt="ElQuatro logo" width="180"></div>
    <div class="hero-heading">      
      <h1 class="title">Do you want to create your own best travel memories?</h1>
      <h2 class="subtitle">Let us help you!</h2>
      <a class="button is-danger is-small">Contact Us</a>
    </div>
    <div class="hero-head">   

      <nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
        <div id="navbarBasicExample" class="navbar-menu">
          <div class="navbar-end">
            <div class="navbar-item">
              <div class="buttons">
                <a class="button is-warning is-small">                    
                  Our Journey                      
                </a> 
              </div>
            </div>
          </div>
        </div>
      </nav>

    </div>
    <div class="hero-body">
      <div class="container">
        <h1 class="title has-text-centered">
          5 Easy Steps
        </h1>
        <div class="columns is-centered is-multiline has-text-centered">
          <div class="column is-2 is-narrow">
            <img src="@@/assets/img/step1.png" alt="step 1" />
            <p>Choose from our destinations</p>
          </div>
          <div class="column is-2 is-narrow">
            <img src="@@/assets/img/step2.png" alt="step 2" />
            <p>We book the hotel</p>
          </div>
          <div class="column is-2 is-narrow">
            <img src="@@/assets/img/step3.png" alt="step 3" />
            <p>We book the plane, ferry and bus tickets</p>
          </div>
          <div class="column is-2 is-narrow">
            <img src="@@/assets/img/step4.png" alt="step 4" />
            <p>We book your tour packages</p>
          </div>
          <div class="column is-2 is-narrow">
            <img src="@@/assets/img/step5.png" alt="step 5" />
            <p>Sit back and relax</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <footer class="footer">
    <div class="content has-text-centered">
      <p>
        We, from <strong>El Quatro</strong> believes that travelling in other places not your own, makes life more exciting.
        It helps you become a better version of your SELF. It pushes you to discover new ideas, perspectives and world views by simply interacting with different people-groups and local culture.
        Moving around unfamiliar places also compels you to be resourceful, street smart and naturally instinctive.
      </p>
      <p>
        Travelling makes the places both playgrounds and your classrooms. Guaranteed you both will have fun at the same time learn your class subjects, first hand.
        The experience becomes personal. The realising becomes personal. And you'll know, no one can ever take it from you. 
      </p>
      <br />
      <h2>Travel with El Quatro</h2>
      <h3>We are sure to make your journey worth your while</h3>
    </div>
  </footer>
</div>
</template>

<script>
import Vue from 'vue'
import Buefy from 'buefy'
import 'buefy/dist/buefy.css'
import '@@/assets/css/style.css'

Vue.use(Buefy)

export default {
  head: {
    title: 'Home page'
  }
}
</script>
