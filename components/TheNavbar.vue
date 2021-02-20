<template>
  <div>
    <b-navbar
      fixed="top"
      type="light"
      variant="light"
      toggleable="lg"
      class="header header-fix"
    >
      <b-navbar-brand to="/">
        <h1 class="nav-header">Kontakt</h1>
      </b-navbar-brand>
      <b-navbar-nav class="ml-lg-5 pos-fix">
        <b-nav-item>
          <the-sidebar></the-sidebar>
        </b-nav-item>
      </b-navbar-nav>
      <b-navbar-toggle
        target="nav-collapse"
        class="btn"
      ></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav right >
        <b-navbar-nav class="ml-lg-5">
          <b-nav-item class="pr-3 nav-item-color" to="/contacts"
            >Contacts</b-nav-item
          >
          <b-nav-item class="pr-3 nav-item-color" to="/add-contact"
            >Add New Contact</b-nav-item
          >
          <b-nav-item class="nav-item-color" to="/calendar"
            >Calendar</b-nav-item
          >
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
.wrapper {
  position: sticky;
  top: 0;
}
.pos-fix {
  position: relative;
  padding: 1rem;
}
.nav-header {
  color: black;
  border-bottom: solid 1px #007bff;
}
.nav-item-color {
  color: black;
}
.res-toggle {
  color: #007bff;
  background-clip: black;
}
</style>