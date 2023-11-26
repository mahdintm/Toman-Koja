<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div>
      <b-navbar toggleable="sm" type="dark" variant="info">
        <b-navbar-brand href="#">Toman</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-form>
              <b-form-input size="sm" class="mr-sm-1" placeholder="Search"></b-form-input>
              <b-button size="sm" class="my-1 my-sm-0" type="submit">Search</b-button>
            </b-nav-form>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
  </header>

  <RouterView />
</template>
<style scoped>
/* @import url('/node_modules/bootstrap/dist/css/bootstrap.css'); */
</style>
