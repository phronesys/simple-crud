<template>
  <div class="container-xl medium-margin-top">
    <h2>New Contact</h2>
    <b-form @submit="onSubmit" @reset="onReset" v-if="show">
      <b-form-group id="input-group-1" label="Name:" label-for="input-1">
        <b-form-input
          id="input-1"
          v-model="form.name"
          placeholder="John Doe"
          required
        ></b-form-input>
      </b-form-group>
      <b-form-group id="input-group-2" label="Ocupation:" label-for="input-2">
        <b-form-input
          id="input-2"
          v-model="form.alias"
          placeholder="Student"
          required
        ></b-form-input>
      </b-form-group>
      <b-form-group
        id="input-group-3"
        label="Email address:"
        label-for="input-3"
      >
        <b-form-input
          id="input-1"
          v-model="form.email"
          type="email"
          placeholder="John@Doe.com"
          required
        ></b-form-input>
      </b-form-group>
      <b-form-group
        id="input-group-4"
        label="Phone:"
        label-for="input-4"
        description="We'll never share your data with anyone else."
      >
        <b-form-input
          id="input-1"
          v-model="form.phone"
          type="phone"
          placeholder="+56912345678"
          required
        ></b-form-input>
      </b-form-group>

      <b-button type="submit" variant="primary">Add</b-button>
      <b-button type="reset" variant="danger">Reset</b-button>
    </b-form>
    <!-- <b-card class="mt-3" header="Form Data Result">
      <pre class="m-0">{{ form }}</pre>
    </b-card> -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        email: "",
        name: "",
        food: null,
        checked: [],
      },
      foods: [
        { text: "Select One", value: null },
        "Carrots",
        "Beans",
        "Tomatoes",
        "Corn",
      ],
      show: true,
    };
  },
  methods: {
    onSubmit(event) {
      event.preventDefault();
      alert(JSON.stringify(this.form));
    },
    onReset(event) {
      event.preventDefault();
      // Reset our form values
      this.form.email = "";
      this.form.name = "";
      this.form.food = null;
      this.form.checked = [];
      // Trick to reset/clear native browser form validation state
      this.show = false;
      this.$nextTick(() => {
        this.show = true;
      });
    },
  },
};
</script>

<style>
</style>