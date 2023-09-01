<script>
export default {
  data() {
    return {
      Courses: [
        {
          course_name: "The Acrylic Painting Academy",
          price: "$18.00",
          lessons: " 4 Lessons",
          students: " 50 Students",
        },
        {
          course_name: "Drawing and Shading: Complete Course",
          price: "$21.00",
          lessons: " 14 Lessons",
          students: " 50 Students",
        },
        {
          course_name: "The Color Theory for Digital Artist",
          price: "$19.00",
          lessons: " 7 Lessons",
          students: " 50 Students",
        },
        {
          course_name: "Ultimate Guide to Digital Sketching for Beginner",
          price: "$35.00",
          lessons: " 14 Lessons",
          students: " 50 Students",
        },
        {
          course_name: "Portrait Drawing The Smart Way",
          price: "$19.00",
          lessons: " 2 Lessons",
          students: " 50 Students",
        },
        {
          course_name: "Mastering Watercolor Painting from Beginner",
          price: "$19.00",
          lessons: " 9 Lessons",
          students: " 50 Students",
        },
        {
          course_name: "The Art & Science of Drawing",
          price: "$25.00",
          lessons: " 4 Lessons",
          students: " 50 Students",
        },
        {
          course_name: "The Colored Pencil Drawing Course",
          price: "$22.00",
          lessons: " 6 Lessons",
          students: " 50 Students",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container">
    <!--Artist Coaching-->
    <div class="ps-5 pe-5">
      <div class="text-center">
        <h3>Artist Coaching</h3>
        <h1>I understand what it takes to create.<br />I can help you with:</h1>
      </div>
      <div class="d-flex mt-5 mb-5">
        <div class="p-3">
          <img
            class="mb-3"
            src="../assets/img/artist-box-image-01.png"
            alt=""
          />
          <h5>Online courses</h5>
          <p>
            Online art coaching now offers you a very powerful way to redesign
            your artist mind
          </p>
        </div>
        <div class="mt-5 p-3">
          <img
            class="mb-3"
            src="../assets/img/artist-box-image-02.png"
            alt=""
          />
          <h5>One to One</h5>
          <p>
            Online art coaching now offers you a very powerful way to redesign
            your artist mind
          </p>
        </div>
        <div class="p-3">
          <img
            class="mb-3"
            src="../assets/img/artist-box-image-03.png"
            alt=""
          />
          <h5>Anywhere</h5>
          <p>
            Online art coaching now offers you a very powerful way to redesign
            your artist mind
          </p>
        </div>
        <div class="mt-5 p-3">
          <img
            class="mb-3"
            src="../assets/img/artist-box-image-04.png"
            alt=""
          />
          <h5>On Time</h5>
          <p>
            Online art coaching now offers you a very powerful way to redesign
            your artist mind
          </p>
        </div>
      </div>
    </div>
    <!--Coach and Mentor-->
    <div
      class="container d-flex justify-content-between align-items-center pe-5 ps-5"
    >
      <div class="text-center">
        <div class="flex-grow-1">
          <div><img src="../assets/img/artist-quote-icon.png" alt="" /></div>
          <div class="ps-5 pe-5">
            <div class="mt-3 mb-5">
              <span class="display-5 fw-bold">
                I coach and mentor<br />
                visual artists, like <br />you, to create Like<br />
                you mean it
              </span>
            </div>
            <h3>Martin Garrix</h3>
          </div>
        </div>
      </div>
      <div class="side-text mb-5">
        <div>
          <div class="mt-5">
            <p>
              As a coach and mentor, my ultimate goal is to motivate visual
              artists toward inspired action. I help you get back on track to
              being the productive, creative, meaningful and authentic artist
              you truly want to be. I support artists in crafting an dliving a
              creative life as well as feeling good about themselves and their
              art.
            </p>
            <p>
              As an artist and an educator for nearly 30 years, I understand
              what it takes to create.
            </p>
          </div>
          <div class="mt-5"><button>Get started today</button></div>
        </div>
      </div>
    </div>
    <!--Youtube Video-->
    <div
      class="distancing-pls position-relative container d-flex justify-content-center align-items-center"
    >
      <div>
        <div>
          <img src="../assets/img/artist-video-poster.jpg" alt="" />
          <img
            class="position-absolute yt-pb"
            src="../assets/img/icon-youtube-play.png"
            alt=""
          />
        </div>
      </div>
    </div>
    <!--Testimonials-->
    <div class="container text-center mb-5 mt-5">
      <h3>Testimonials</h3>
      <h1>Why do people love me?</h1>
    </div>
    <!--Slider-->
    <div>
      <div>
        <div class="m-5">
          <div>
            <h5>It's a choice of quality for people with special needs</h5>
            <p class="font-size-small">
              I'm a very strict person so I require everything to be<br />
              organized and neat. Then, I'll be able to make things<br />
              right and shine. MaxCoach guys just got me.
            </p>
          </div>
          <div class="d-flex">
            <div>
              <img
                class="testimonial-pic"
                src="../assets/img/artist-testimonial-avatar-01.jpg"
                alt=""
              />
            </div>
            <div>
              <span>Florence Themes</span><br />
              <span>/Multimedia Admin</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!--Artist Coaching 2-->
    <div class="mb-5 mt-5">
      <div class="text-center">
        <h3>Artist Coaching</h3>
        <h1>Latest Online Courses</h1>
      </div>
      <div class="d-flex flex-wrap m-auto mb-5">
        <div class="course-card m-3" v-for="(course, i) in this.Courses">
          <div class="mb-2">
            <img
              class="course-img"
              :src="`src/assets/img/artist-course-0${i + 1}-480x480.jpg`"
              alt="course image"
            />
          </div>
          <div class="course-infos ms-3">
            <div class="mt-2 mb-2">
              <span>{{ course.price }}</span>
              <h5>{{ course.course_name }}</h5>
            </div>
            <div>
              <span
                ><i class="fa-solid fa-list-ul"></i>{{ course.lessons }}
                <i class="fa-regular fa-user"></i>{{ course.students }}</span
              >
            </div>
          </div>
        </div>
      </div>
      <div class="d-flex justify-content-center">
        <button>
          View all courses <i class="fa-solid fa-arrow-right-long"></i>
        </button>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.side-text {
  font-size: 1.2rem;
  width: 50%;
}

.distancing-pls {
  margin-top: 150px;
  margin-bottom: 80px;
}

.yt-pb {
  left: 46%;
  bottom: 43%;
}

.course-card {
  width: calc((100% / 4) - 32px);
  img {
    height: 100%;
    width: 100%;
  }
  .course-infos {
    width: 85%;
  }

  .testimonial-pic {
    max-width: 40px;
    max-height: 40px;
  }
}
</style>
