<template>
  <div>
    <b-navbar type="dark" variant="dark" sticky toggleable="lg">
      <b-navbar-brand>My Contacts</b-navbar-brand>
      <b-navbar-nav class="ml-lg-5">
        <b-nav-item>
          <the-sidebar></the-sidebar>
        </b-nav-item>
      </b-navbar-nav>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-lg-5">
          <b-nav-item>Link 1</b-nav-item>
          <b-nav-item>Link 2</b-nav-item>
          <b-nav-item disabled>Disabled</b-nav-item>
        </b-navbar-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown text="User" right>
            <b-dropdown-item>Log in</b-dropdown-item>
            <b-dropdown-item>Logout</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
import TheSidebar from "./TheSidebar.vue";
export default {
  components: { TheSidebar },
};
</script>

<style>
</style>