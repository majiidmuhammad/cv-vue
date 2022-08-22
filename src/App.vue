<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Personal from './components/Personal.vue'
</script>

<template>

<nav class="navbar navbar-expand-lg navbar-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="/">Personal</a>
        </li>
        <li class="nav-item">
          <a class="nav-link active" href="/skill">Skill</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/WhatsApp Image 2022-08-16 at 13.44.34.jpeg" width="125" height="160" />

    <div class="wrapper">
      <div class="text">
        <Personal msg="Majiid Muhammad" />
      </div>

    </div>
  </header>

  <RouterView />
</template>

<style scoped>

.navbar {
  background-color: orange;
  border-radius: 15px;
}

.text {
  color: black;
  margin-top: -30px;
}

.nav {
  margin-left: 30rem;
}

/* .nav h1 {
  display: flex; */
/* } */

header {
  line-height: 1.5;
  max-height: 100vh;
  margin-top: 30px;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  border-radius: 15px;
}

/* nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
} */

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
    margin-bottom: 50px;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  /* nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  } */
}
</style>
