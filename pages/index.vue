<template>
  <div class="bg-img shadow">
    <!-- <h2 class="ml-auto">Add your clients</h2> -->
    <div class="container custom-p-20">
      <div class="row">
        <div class="col-lg-12 text-left text-dark">
          <h1 class="mt-5 display-3 display-small ">
            Add your clients 
          </h1>
          <p class="lead display-5 display-very-small">
            Free up more time by managing your clients smartly
          </p>
          <b-button pill class="text-light shadow" variant="primary"
            >Get started!</b-button
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.bg-img {
  background-image: url("../assets/professional-solution.jpg");
  background-color: #edefee;
  height: 100%;
  background-position: center;
  background-size: 100%;
  padding: 3rem 0;
  background-repeat: no-repeat;
}
.header {
  box-shadow: 0rem 1rem 2rem rgba(0, 0, 0, 0.4);
}

.custom-p-20 {
  padding: 10rem;
  margin-top: 6rem;
}
.shadow {
  box-shadow: 0rem 1rem 2rem rgba(0, 0, 0, 0.4);
}
@media (max-width: 1024px) {
  .bg-img {
    /* background-color: #edefee; */
    height: 100%;
    background-position: center;

    padding-bottom: 5rem;
    background-repeat: no-repeat;
  }
  .custom-p-20 {
    padding: 5rem;
    margin: 1rem 0rem;
  }
  .display-small {
    font-size: 3rem;
  }
  .display-very-small {
    font-size: 1rem;
  }
}
@media (max-width: 766px) {
  .bg-img {
    background-size: 150%;
    background-position: cover;
    padding: 3rem 4rem;
  }
  .custom-p-20 {
    padding: 5rem 0rem;

    margin-top: 8rem;
  }
  .display-very-small {
    font-size: 1rem;
  }
}
@media (max-width: 600px) {
  .bg-img {
    background-position: cover;
    padding: 1rem;
  }
  .custom-p-20 {
    padding: 4rem 2rem;

    margin-top: 4rem;
  }
  .display-small {
    font-size: 2rem;
  }
  .display-very-small {
    font-size: 1rem;
    width: 75%;
  }
}

@media (max-width: 425px) {
  .bg-img {
    height: 100%;
    background-position: center;
    background-size: 200%;
    padding: 0;
    background-repeat: no-repeat;
  }
  .custom-p-20 {
    padding: 2rem;
    margin-top: 10rem;
  }
  .display-small {
    font-size: 2rem;
  }
  .display-very-small {
    font-size: 1rem;
    width: 75%;
  }
  .header {
    display: block;
    text-align: center;
  }
  .res-toggle {
    width: 100%;
    padding: 0rem 1rem;
  }
}
</style>
