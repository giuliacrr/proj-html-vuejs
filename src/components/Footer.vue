<script>
export default {};
</script>

<template>
  <div>
    <!--Newsletter-->
    <div class="bg-primary pt-4 pb-4">
      <div
        class="container d-flex text-white justify-content-center align-items-center"
      >
        <div class="text-end get-in-touch">
          <span>
            Newsletter to get<br />
            in touch
          </span>
        </div>
        <div>
          <div
            class="d-flex d-flex align-items-center input-border"
            tabindex="1"
          >
            <input type="email" placeholder="Your e-mail" />
            <span class="send-btn"
              ><i class="fa-solid fa-arrow-right-long"></i
            ></span>
          </div>
        </div>
      </div>
    </div>
    <!--Newsletter End-->
    <!--Footer-->
    <div class="d-flex pt-5 pb-5 container justify-content-between">
      <!--Address-->
      <div class="me-5">
        <h6>Address</h6>
        <div class="mt-2 mb-2">
          <span class="footer-span"
            >382 NE 191st St # 87394 Miami, FL 33179-3899</span
          >
        </div>
        <div class="mt-2 mb-2">
          <span class="footer-span"
            >+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</span
          >
        </div>
        <div class="mt-2 mb-2">
          <span class="footer-span">support@maxcoach.com</span>
        </div>
        <div class="d-flex align-items-center">
          <div class="me-3">
            <a href=""><i class="fa-brands fa-square-facebook"></i></a>
          </div>
          <div class="me-3">
            <a href=""><i class="fa-brands fa-square-x-twitter"></i></a>
          </div>
          <div class="me-3">
            <a href=""><i class="fa-brands fa-square-instagram"></i></a>
          </div>
          <div class="me-3">
            <a href=""><i class="fa-brands fa-linkedin"></i></a>
          </div>
        </div>
      </div>
      <!--Explore-->
      <div>
        <h6>Explore</h6>
        <ul>
          <li><a href="">Start here</a></li>
          <li><a href="">Success story</a></li>
          <li><a href="">Blog</a></li>
          <li><a href="">Courses</a></li>
          <li><a href="">Contact us</a></li>
        </ul>
      </div>
      <!--Information-->
      <div class="me-5">
        <h6>Information</h6>
        <ul>
          <li><a href="">Start here</a></li>
          <li><a href="">Success story</a></li>
          <li><a href="">Blog</a></li>
          <li><a href="">Courses</a></li>
          <li><a href="">Contact us</a></li>
        </ul>
      </div>
      <!--Instagram-->
      <div class="me-5">
        <h6>
          Instagram
          <a
            href="https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUXbmV2ZXIgZ29ubmEgZ2l2ZSB5b3UgdXA%3D"
            >@maxcoach</a
          >
        </h6>
        <div class="d-flex">
          <div class="instagram">
            <img
              src="../assets/img/120084500_197897808368764_8114555493043279565_n.jpg"
              alt="instapic"
            />
          </div>
          <div class="instagram">
            <img
              src="../assets/img/120012142_177596140500760_8623485824101406058_n.jpg"
              alt="instapic"
            />
          </div>
          <div class="instagram">
            <img
              src="../assets/img/120099363_364334431619755_7198812647386067017_n.jpg"
              alt="instapic"
            />
          </div>
        </div>
      </div>
    </div>
    <!--Footer End-->
  </div>
</template>

<style lang="scss" scoped>
.get-in-touch {
  font-size: 2rem;
  margin-right: 100px;
}
.send-btn {
  margin-left: -20px;
}
input {
  border: 1px solid transparent;
  border-bottom-color: rgb(184, 184, 184);
  background-color: transparent;
  color: white;
  font-size: 1.6rem;
  border-radius: 0;
  width: 500px;
}

input:focus {
  border-bottom-color: rgb(255, 255, 255);
}

input:focus-visible {
  outline: none;
}

::placeholder {
  color: white;
  font-size: 1.6rem;
}

i {
  font-size: 1.4rem;
}

ul {
  list-style: none;
}

.footer-span {
  font-size: 0.85rem;
}

ul {
  padding: 0;
  li {
    margin-top: 10px;
    margin-bottom: 10px;
  }
  a {
    text-decoration: none;
  }
}

.instagram {
  margin-left: 5px;
  margin-right: 5px;
  width: calc((100% / 3) - 10px);
  height: auto;
  img {
    width: 120px;
  }
}
</style>
