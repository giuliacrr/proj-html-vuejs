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
    <div class="ps-5 pe-5 mt-5 mb-5">
      <div class="text-center">
        <h1 class="custom-title-mills">Artist Coaching</h1>
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
    <div class="mt-5 mb-5 l-gray">
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
              <h1 class="custom-title-mills">Martin Garrix</h1>
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
            <div class="mt-5">
              <button class="orange-button fw-bold pt-3 pb-3 ps-5 pe-5">
                Get started today
              </button>
            </div>
          </div>
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
      <h1 class="custom-title-mills">Testimonials</h1>
      <h1>Why do people love me?</h1>
    </div>
    <!--Slider-->
    <!--Artist Coaching 2-->
    <div class="mb-5 mt-5">
      <div class="text-center">
        <h1 class="custom-title-mills">Artist Coaching</h1>
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
          <div class="course-infos ms-3 bg-light p-2">
            <div class="mt-2 mb-2">
              <span class="link-orange fw-bold">{{ course.price }}</span>
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
    <!--Articles and Tips-->
    <div class="mt-5 mb-5">
      <div class="text-center mt-5 mb-5">
        <h1 class="custom-title-mills">Articles and Tips</h1>
        <h1>Latest From The Blog</h1>
      </div>
      <div>
        <div>
          <div class="d-flex mb-5 justify-content-center">
            <!--Left one-->
            <div class="course-blog left-article blog-img small-post-descr">
              <div class="mb-2">
                <img
                  style="width: 250px; height: 200px"
                  src="../assets/img/120084500_197897808368764_8114555493043279565_n.jpg"
                  alt="blog image"
                />
              </div>
              <div class="course-infos ms-3">
                <div class="mt-2 mb-2">
                  <span>ARTIST</span>
                  <h5>Brush Strokes Energize Trees in Paintings</h5>
                </div>
                <div>
                  <span
                    ><i class="fa-regular fa-calendar"></i> May 15, 2020</span
                  ><br />
                  <span><i class="fa-regular fa-eye"></i> 1,805 views</span>
                </div>
              </div>
            </div>

            <!--Middle One-->
            <div>
              <div class="position-relative">
                <img src="../assets/img/artist-blog-02-500x680.jpg" alt="" />
                <div class="position-absolute big-post-descr text-white p-5">
                  <div class="mt-ow">
                    <span>ARTIST</span>
                    <h1>Connection Between Self-Portraits and Identity</h1>
                    <div>
                      <span
                        ><i class="fa-regular fa-calendar"></i> May 15,
                        2020</span
                      ><br />
                      <span><i class="fa-regular fa-eye"></i> 1,805 views</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <!--Right one-->
            <div class="course-blog small-post-descr right-article">
              <div class="mb-2">
                <img
                  style="width: 250px; height: 200px"
                  src="../assets/img/artist-blog-01-480x356.jpg"
                  alt="blog image"
                />
              </div>
              <div class="course-infos blog-img ms-3">
                <div class="mt-2 mb-2">
                  <span>ARTIST</span>
                  <h5>Pocket-Sized Notebooks Hold Miniature Paintings</h5>
                </div>
                <div>
                  <span
                    ><i class="fa-regular fa-calendar"></i> May 15, 2020</span
                  ><br />
                  <span><i class="fa-regular fa-eye"></i> 1,688 views</span>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="text-center">
          <span
            >Get into details now?
            <a class="link-orange" href=""
              >View all posts
              <i class="fa-solid fa-arrow-right-long link-orange"></i></a
          ></span>
        </div>
      </div>
    </div>
    <!--Upcoming Events-->
    <div class="mt-5 mb-5">
      <div class="text-center">
        <h1 class="custom-title-mills">Upcoming Events</h1>
        <h1>Let's work Together</h1>
      </div>
      <!--First row-->
      <div class="container d-flex justify-content-center mt-5">
        <div class="d-flex">
          <!--Event one-->
          <div class="events d-flex">
            <div>
              <img
                src="../assets/img/artist-event-04-250x300.jpg"
                alt="artist event"
              />
            </div>
            <div class="d-flex justify-content-center align-items-center p-5">
              <div>
                <div>
                  <span>APR 22, 2021</span>
                  <h5>Storytelling Workshop</h5>
                </div>
                <div>
                  <span
                    ><i class="fa-solid fa-location-dot"></i> Texas, US</span
                  >
                </div>
              </div>
            </div>
          </div>
          <!--Event two-->
          <div class="events d-flex ms-4">
            <div>
              <img
                style="width: 250px; height: 300px"
                src="../assets/img/artist-event-03-250x300.jpg"
                alt="artist event"
              />
            </div>
            <div class="d-flex justify-content-center align-items-center p-5">
              <div>
                <div>
                  <span>OCT 10, 2020</span>
                  <h5>Painting Art Contest 2020</h5>
                </div>
                <div>
                  <span
                    ><i class="fa-solid fa-location-dot"></i> New York, US</span
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
        <div></div>
      </div>
      <!--Second row-->
      <div class="container d-flex justify-content-center mt-5">
        <!--Event three-->
        <div class="d-flex">
          <div class="d-flex justify-content-center align-items-center p-5">
            <div class="text-end">
              <div>
                <span>NOV 23, 2020</span>
                <h5>International Art Fair 2020</h5>
              </div>
              <div>
                <span
                  ><i class="fa-solid fa-location-dot"></i> Hamburg,
                  Germany</span
                >
              </div>
            </div>
          </div>
          <div>
            <img
              style="width: 250px; height: 300px"
              src="../assets/img/artist-event-02-250x300.jpg"
              alt="artist event"
            />
          </div>
        </div>
        <!--Event four-->
        <div class="d-flex">
          <div class="d-flex justify-content-center align-items-center p-5">
            <div class="text-end">
              <div>
                <span>DEC 15, 2020</span>
                <h5>
                  Street Performance: Call for<br />
                  Artist
                </h5>
              </div>
              <div>
                <span
                  ><i class="fa-solid fa-location-dot"></i> Illinois, US</span
                >
              </div>
            </div>
          </div>
          <div>
            <img
              style="width: 250px; height: 300px"
              src="../assets/img/artist-event-01-250x300.jpg"
              alt="artist event"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.border-red {
  border: 1px dashed red;
}

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
    border: 1px dashed $orange;
  }
}

.testimonial-img {
  width: 50px;
  height: auto;
  border-radius: 50%;
}

.big-post-descr {
  top: 0%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.2);
}
.small-post-descr {
  width: 300px;
}
.mt-ow {
  margin-top: 350px;
}

.course-blog {
  width: 250px;
}
.left-article {
  margin-top: 200px;
  margin-right: 60px;
}
.right-article {
  margin-top: 80px;
  margin-left: 60px;
}

.events {
  width: calc(100% / 2);
}
</style>
