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
  <div class="fb">
    <div>
      <div
        class="l-gray d-flex justify-content-center align-items-center pt-2 pb-2"
      >
        <div>
          <span>Starts TOMORROW! Our biggest event of the year... </span>
        </div>
        <div class="ms-4">
          <span class="fw-bold"
            ><i class="fa-regular fa-clock"></i> 00 : 00 : 00 : 00</span
          >
        </div>
        <div class="ms-5">
          <button class="orange-button fw-bold">Get ticket</button>
        </div>
      </div>
    </div>
    <!--Fascia bassa-->
    <div class="pt-3 pb-3 bg-light">
      <div class="container d-flex justify-content-between align-items-center">
        <div class="text-dgrey"><strong>Max</strong>Coach</div>
        <!--Center menu with dropdowns-->
        <div class="d-flex">
          <!--Home-->
          <div class="dropdown" v-for="item in dropdowns">
            <button
              class="btn"
              type="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              <span class="nav-dd-hover"
                >{{ item }} <i class="fa-solid fa-chevron-down"></i
              ></span>
            </button>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#">Action</a></li>
              <li><a class="dropdown-item" href="#">Another action</a></li>
              <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul>
          </div>
        </div>
        <div>
          <div class="d-flex align-items-center">
            <div class="me-3">
              <a href=""
                ><i class="nav-dd-hover fa-brands fa-square-facebook"></i
              ></a>
            </div>
            <div class="me-3">
              <a href=""
                ><i class="nav-dd-hover fa-brands fa-square-x-twitter"></i
              ></a>
            </div>
            <div class="me-3">
              <a href=""
                ><i class="nav-dd-hover fa-brands fa-square-instagram"></i
              ></a>
            </div>
            <div class="me-3">
              <a href=""><i class="nav-dd-hover fa-brands fa-linkedin"></i></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!--Herosection-->
  <div class="pt-5 pb-5 hero-s">
    <div
      class="d-flex justify-content-center align-items-center container mb-5"
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
        <button class="orange-button fw-bold pt-3 pb-3 ps-5 pe-5 mt-5">
          Get started today
        </button>
      </div>
      <!--Pics on the right-->
      <div><img src="../assets/img/artist-hero-image-04.jpg" alt="guy" /></div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.fb {
  z-index: 1;
  position: fixed;
  top: 0;
  width: 100%;
}
.fa-chevron-down {
  font-size: 0.8rem;
}
.position-absolute {
  bottom: -20%;
  left: -35%;
}
.text-dgrey {
  font-size: 2rem;
}
</style>
