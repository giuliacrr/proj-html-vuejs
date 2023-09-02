<script>
export default {
  data() {
    return {
      dropdowns: ["Home", "Pages", "Courses", "Featurers", "Blog", "Shop"],
    };
  },
};
</script>

<template>
  <!--Fascia alta-->
  <div>
    <div class="d-flex justify-content-center">
      <div><span>Starts TOMORROW! Our biggest event of the year...</span></div>
      <div><span>orologio</span></div>
      <div><button>Get ticket</button></div>
    </div>
  </div>
  <!--Fascia bassa-->
  <div>
    <div class="container d-flex justify-content-between align-items-center">
      <div>MaxCoach</div>
      <!--Center menu with dropdowns-->
      <div class="d-flex">
        <!--Home-->
        <div class="dropdown" v-for="item in dropdowns">
          <button
            class="btn btn-secondary dropdown-toggle"
            type="button"
            data-bs-toggle="dropdown"
            aria-expanded="false"
          >
            {{ item }}
          </button>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </div>
      </div>
      <div>Socials</div>
    </div>
  </div>
  <!--Herosection-->
  <div
    class="d-flex justify-content-center align-items-center container mt-5 mb-5"
  >
    <!--Pics on the left-->
    <div class="position-relative ms-5">
      <img src="../assets/img/artist-hero-image-02.jpg" alt="??" />
      <img
        class="position-absolute"
        src="../assets/img/artist-hero-image-01.jpg"
        alt="monke"
      />
    </div>
    <!--Center writing-->
    <div class="text-center ms-5 me-5">
      <h1 class="custom-title-mills">Hello, I'm Martin</h1>
      <h1>
        Artist Coaching and Mentoring<br />
        Might Be for You.
      </h1>
      <button>Get started today</button>
    </div>
    <!--Pics on the right-->
    <div><img src="../assets/img/artist-hero-image-04.jpg" alt="guy" /></div>
  </div>
</template>

<style lang="scss" scoped>
.position-absolute {
  bottom: -20%;
  left: -35%;
}
</style>
