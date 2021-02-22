<template>
  <div>
    <div class="container-fluid medium-margin-top">
      <div>
        <ul class="contact-list">
          <li class="contact" v-for="contact in contactList" :key="contact">
            <h4>
              {{ contact.name }}
            </h4>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  // dummy data, data will be manage in the store
  data() {
    return {
      contactList: [
        {
          name: "Kira",
          alias: "my doggo",
          mail: "dog@mail.com",
          phone: "+56912345678",
        },
        {
          name: "Daniel",
          alias: "El creador de esta página bien cutre",
          mail: "dd@mail.com",
          phone: "+56912345678",
        },
        {
          name: "User",
          alias: "just a random user",
          mail: "user@mail.com",
          phone: "+56912345678",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
ul {
  padding: 0;
  list-style-type: none;
}
.contact-list {
  display: flex;
  flex-wrap: wrap;
  list-style: none;
  margin: 0;
}
.contact {
  border-radius: 10px;
  margin: 1rem;
  padding: 1rem;
  text-align: center;
  width: 250px;
  height: 250px;

  box-shadow: 0rem 0rem 1rem rgba(#000000, 0.6);
}
</style>