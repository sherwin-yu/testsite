<template>
  <div id="app">
    <div>
      <b-navbar toggleable="lg" type="light">
        <router-link to="/">
          <b-navbar-brand>Kiana Cao</b-navbar-brand>
        </router-link>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-navbar-nav>
              <b-nav-item>
                <router-link class="nav-link" to="/work">WORK</router-link>
              </b-nav-item>
              <b-nav-item>
                <router-link class="nav-link" to="/about">ABOUT</router-link>
              </b-nav-item>
              <b-nav-item>
                <router-link class="nav-link" to="/contact">CONTACT</router-link>
              </b-nav-item>
            </b-navbar-nav>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
    <router-view />
  </div>
</template>

<!-- Your global styles here -->
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.nav-link {
  text-decoration: none;
}
</style>
