<template>
  <div>
    <div class="bg-img shadow mb-5">
      <!-- <h2 class="ml-auto">Add your clients</h2> -->
      <div class="container custom-p-20">
        <div class="row">
          <div class="col-lg-12 text-left text-dark">
            <h1 class="mt-5 display-3 display-small">
              Start adding your clients
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
    <div class="container-fluid medium-margin-top">
      <h2 class="display-2 text-center text-primary">We focus on solutions</h2>
      <h3 class="display-5 text-center">
        here it goes the sub title where we describe the main suquis truquis
      </h3>
      <div class="row text-center card-box">
        <div class="col-sm">
          <div class="card card__feature">
            <div class="card-body bg-img-2 text-light">
              <h3 class="card-title">Free!</h3>
              <p class="card-text">
                Some quick example text to build on the card title and make up
                the bulk of the card's content.
              </p>
            </div>
            <ul class="list-group list-group-flush">
              <li class="list-group-item">Dapibus ac facilisis in</li>
              <li class="list-group-item">Vestibulum at eros</li>
            </ul>
            <div class="card-body">
              <a href="#" class="btn btn-outline-primary mx-2">Card link</a>
              <a href="#" class="btn btn-primary mx-2">Another link</a>
            </div>
          </div>
        </div>
        <div class="col-sm">
          <div class="card card__feature">
            <div class="card-body bg-img-3 text-light">
              <h3 class="card-title">Enterprise</h3>
              <p class="card-text">
                Some quick example text to build on the card title and make up
                the bulk of the card's content.
              </p>
            </div>
            <ul class="list-group list-group-flush">
              <li class="list-group-item">Dapibus ac facilisis in</li>
              <li class="list-group-item">Vestibulum at eros</li>
            </ul>
            <div class="card-body">
              <a href="#" class="btn btn-outline-primary mx-2">Card link</a>
              <a href="#" class="btn btn-primary mx-2">Another link</a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="bg-primary p-1 brightness">
        <b-embed
          type="iframe"
          aspect="16by9"
          src="https://youtube.com/embed/dQw4w9WgXcQ"
          allowfullscreen
        ></b-embed>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.brightness{
  box-shadow: 1rem 1rem 2rem black;
  border-radius: 5px;
  filter: brightness(0);
  transition: all 1s ease-in;
  &:hover {
    filter: brightness(1);
  }
}
.card-box {
  max-width: 80%;
  margin: 8rem auto;
}

.card__feature {
  border-radius: 10px;
  height: 25rem;
  box-shadow: 0rem 1rem 1rem #007bffbd;
  transition: 1s ease;
  overflow: hidden;
  &:hover {
    transform: translateY(-1rem);
    box-shadow: 0rem 1rem 4rem #007bffbd;
  }
  &:hover .bg-img-2 {
    opacity: 1;
  }
  &:hover .bg-img-3 {
    opacity: 1;
  }
}
.demo-try {
  text-align: center;
  background-color: rgba(0, 0, 0, 0.4);
  border-radius: 5px;
  &__button {
    position: relative;
    margin: 1rem;
  }
}
.bg-text {
  text-align: center;
  padding: 1rem;
  padding-bottom: 0;
  font-size: 5vw;
  &-2 {
    text-align: center;

    padding: 1rem;
    font-size: 3vw;
  }
}
.bg-img {
  background-image: url("../assets/professional-solution.jpg");
  background-color: #edefee;
  height: 100%;
  background-position: center;
  background-size: 100%;
  padding: 3rem 0;
  background-repeat: no-repeat;
  &-2 {
    background-image: url("../assets/to-work.jpeg");
    background-position: center;
    opacity: 0.3;
    background-size: cover;
    transition: 1s ease;
  }
  &-3 {
    background-image: url("../assets/backendguys.jpg");
    background-position: center;
    opacity: 0.3;
    background-size: cover;
    transition: 1s ease;
  }
}
.header {
  box-shadow: 0rem 0rem 1rem rgba(0, 0, 0, 0.4);
}

.custom-p-20 {
  padding: 5rem;
  margin-top: 6rem;
}
.shadow {
  box-shadow: 0rem 1rem 2rem rgba(0, 0, 0, 0.4);
}
.small-margin-top {
  margin-top: 5rem;
}
.medium-margin-top {
  margin-top: 10rem;
}
.big-margin-top {
  margin-top: 20rem;
}
.bigger-margin-top {
  margin-top: 30rem;
}
.ultra-margin-top {
  margin-top: 50rem;
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
@media (max-width: 776px) {
  .card-box {
    max-width: 100%;
    margin: 2rem auto;
  }
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
