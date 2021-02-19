<template>
  <div>
    <b-navbar type="dark" variant="dark" sticky toggleable="lg">
      <b-navbar-brand to="/">My Contacts</b-navbar-brand>
      <b-navbar-nav class="ml-lg-5">
        <b-nav-item>
          <the-sidebar></the-sidebar>
        </b-nav-item>
      </b-navbar-nav>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-lg-5" variant="success">
          <b-nav-item to="/contacts">Contacts</b-nav-item>
          <b-nav-item to="/add-contact">Add New Contact</b-nav-item>
          <b-nav-item to="/calendar">Calendar</b-nav-item>
        </b-navbar-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown text="User" right>
            <b-dropdown-item to="/user">User Details</b-dropdown-item>
            <b-dropdown-item to="/login">Login</b-dropdown-item>
            <b-dropdown-item to="/">Logout</b-dropdown-item>
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