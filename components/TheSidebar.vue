<template>
  <div>
    <b-button pill v-b-toggle.sidebar-1 variant="primary"
      >Upcoming Events</b-button
    >
    <b-sidebar
      id="sidebar-1"
      title="Next meeting"
      shadow
      bg-variant="dark"
      text-variant="light"
    >
      <template #default="{ hide }">
        <div class="p-3">
          <h4 id="sidebar-no-header-title">Kira</h4>
          <p>
            Mi perro me observa mientras escribo código, esperando la ocación de
            ir a pasear o de comer algo "rico" nuevo.
          </p>
          <nav class="mb-1">
            <b-nav vertical>
              <b-nav-item active @click="hide">15:30 - 16:00</b-nav-item>
              <b-nav-item>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="16"
                  height="16"
                  fill="currentColor"
                  class="bi bi-geo-alt-fill mr-2 mb-1"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z"
                  />
                </svg>
                <a href="https://www.google.cl/maps" target="_blank">
                  The Direction, 69
                </a>
              </b-nav-item>
            </b-nav>
          </nav>
          <b-button pill variant="outline-primary" class="mb-3 float-right"
            ><svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-pencil-square"
              viewBox="0 0 16 16"
            >
              <path
                d="M15.502 1.94a.5.5 0 0 1 0 .706L14.459 3.69l-2-2L13.502.646a.5.5 0 0 1 .707 0l1.293 1.293zm-1.75 2.456l-2-2L4.939 9.21a.5.5 0 0 0-.121.196l-.805 2.414a.25.25 0 0 0 .316.316l2.414-.805a.5.5 0 0 0 .196-.12l6.813-6.814z"
              />
              <path
                fill-rule="evenodd"
                d="M1 13.5A1.5 1.5 0 0 0 2.5 15h11a1.5 1.5 0 0 0 1.5-1.5v-6a.5.5 0 0 0-1 0v6a.5.5 0 0 1-.5.5h-11a.5.5 0 0 1-.5-.5v-11a.5.5 0 0 1 .5-.5H9a.5.5 0 0 0 0-1H2.5A1.5 1.5 0 0 0 1 2.5v11z"
              /></svg
          ></b-button>
          <b-button
            pill
            to="/details"
            variant="primary"
            class="px-5"
            @click="hide"
            >Details</b-button
          >
        </div>
      </template>
    </b-sidebar>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>