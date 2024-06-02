<template>
  <header>
    <div class="logo">
      <i class="ri-file-paper-2-line ri-xl"></i>
    </div>
    <ul class="options">
      <li>Home</li>
      <li>Features</li>
      <li>Exams</li>
      <li>Aboutus</li>
      <li>Contact</li>
      <li class="user">login</li>
      <li class="user">SignUp</li>
    </ul>
  </header>
  <section>
    <div class="part1">
      <div class="content">
        <span>India's First</span>
        <p>
          Test Preparation <br />Platform directly by <br />
          <span>Top Educators & Institutes</span>
        </p>
        <h5>Get 100% ready for final exam with best online mock test series</h5>
        <button class="user">Get started</button>
      </div>

      <div class="img-container">
        <img
          src="https://png.pngtree.com/png-clipart/20240318/original/pngtree-3d-render-student-with-sitting-study-in-classroom-png-image_14619806.png"
          alt="student"
          loading="lazy"
        />
      </div>
    </div>
    <div class="part2">
      <div class="cont">
        <div class="line-height"></div>
        <div class="line1">
          <div class="arrow"></div>
          <div class="line">
            <img
              src="https://testkart.in/_next/static/media/icon-1.d8596410.svg"
              alt="img"
            />
            <p>Prepare in real exam like scenario</p>
          </div>
        </div>
        <div class="line1">
          <div class="arrow"></div>
          <div class="line">
            <img
              src="https://testkart.in/_next/static/media/icon-1.d8596410.svg"
              alt="img"
            />
            <p>Prepare in real exam like scenario</p>
          </div>
        </div>
        <div class="line1">
          <div class="arrow"></div>
          <div class="line">
            <img
              src="https://testkart.in/_next/static/media/icon-1.d8596410.svg"
              alt="img"
            />
            <p>Prepare in real exam like scenario</p>
          </div>
        </div>
        <div class="line1">
          <div class="arrow"></div>
          <div class="line">
            <img
              src="https://testkart.in/_next/static/media/icon-1.d8596410.svg"
              alt="img"
            />
            <p>Prepare in real exam like scenario</p>
          </div>
        </div>
      </div>
      <div class="img-container">
        <img
          src="https://testkart.in/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fabout.c7780250.png&w=1080&q=75"
          alt="student"
          loading="lazy"
        />
      </div>
      <button class="btn">join now</button>
    </div>
    <div class="part3">
      <h2>Why Students Love Us?</h2>
      <div class="card-container">
        <div class="card" v-for="i in 10" :key="i">
          <img
            src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTa3jmGPWiguMraTQ_vW0VXwY9L9diO25AX0Q&s"
            alt=""
          />
          <div class="content">
            <div class="info">
              <b>javascript</b>
              <p>revise your learning</p>
            </div>
            <button class="btn">learn</button>
          </div>
        </div>
      </div>
    </div>
    <div class="part4">
      <h2>Features!</h2>
      <ul class="list">
        <li>
          <img
            src="https://testkart.in/_next/image?url=%2Fassets%2Fimages%2FListing.png&w=64&q=75"
            alt="logo"
          />
          <b>Set Your Own Price</b>
          <i class="ri-sparkling-line icon"></i>
        </li>
        <li>
          <img
            src="https://testkart.in/_next/image?url=%2Fassets%2Fimages%2Ffree-test-series.png&w=64&q=75"
            alt="logo"
          />
          <b>List Test Series For FREE</b>
          <i class="ri-sparkling-line icon"></i>
        </li>
        <li>
          <img
            src="https://testkart.in/_next/image?url=%2Fassets%2Fimages%2Fall-over-india.png&w=64&q=75"
            alt="logo"
          />
          <b>Access Our Service from anywhere</b>
          <i class="ri-sparkling-line icon"></i>
        </li>
      </ul>
    </div>
  </section>
  <footer>
    <div class="footer">
      <div class="first1">
        <div class="logo">
          <i class="ri-file-paper-2-line ri-xl"></i>
        </div>
        <div class="content">
          Lorem ipsum dolor, sit amet <br />consectetur adipisicing elit.
          <br />Temporibus distinctio error itaque <br />
          voluptate tenetur quasi <br />excepturi voluptates.
        </div>
        <div class="links">
          <i class="ri-facebook-line ri-xl"></i>
          <i class="ri-twitter-line ri-xl"></i>
          <i class="ri-instagram-line ri-xl"></i>
          <i class="ri-linkedin-fill ri-xl"></i>
        </div>
      </div>
      <div class="first1">
        <div class="head">top languages</div>
        <li>javascript</li>
        <li>python</li>
        <li>c++</li>
        <li>java</li>
      </div>
      <div class="first1">
        <div class="head">Quick Links</div>
        <li>Home</li>
        <li>features</li>
        <li>Exams</li>
        <li>Contact</li>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: "LandingPage",
  data() {
    return {};
  },
};
</script>
<style scoped lang="scss">
header {
  padding: 2rem 10rem;
  color: black;
  @include flex(flex, row, center, space-between);
  border-bottom: 1px solid #eee;
  .logo {
    height: 50px;
    width: 50px;
    border-radius: 50%;
    @include flex(flex, row, center, center);
    background-color: whitesmoke;
    i {
      color: $background-color;
    }
  }
  ul {
    list-style: none;
    cursor: pointer;
    @include flex(flex, row, center, space-between, 1.5rem);
  }
}
section > .part1 {
  max-height: 100%;
  min-height: 90vh;
  padding: 4rem 10rem;
  @include flex(flex, row, center, space-between, 1.5rem);
  .content {
    @include flex(flex, column, flex-start, space-between, 0.9rem);
    span {
      color: #c56376;
      font-size: 28px;
      font-weight: 600;
      text-transform: capitalize;
    }
    p {
      margin-top: 1rem;
      font-size: 53px;
      color: black;
      font-family: sans-serif;
      span {
        color: #c56376;
        font-size: 54px;
        font-weight: 600;
        text-transform: capitalize;
      }
    }
    h5 {
      font-size: 18px;
      margin-top: 1rem;
      padding: 0.1rem 0.2rem;
      opacity: 0.8;
      font-weight: 500;
    }
  }
  .img-container {
    width: 40%;
    img {
      height: 80%;
      width: 100%;
    }
  }
}
section > .part2 {
  position: relative;
  max-height: 100%;
  min-height: 90vh;
  padding: 4rem 10rem;
  @include flex(flex, row-reverse, center, space-between, 0);
  .cont {
    position: relative;
    @include flex(flex, column, center, space-between, 1rem);
    .line-height {
      position: absolute;
      height: 450px;
      background-color: red;
      right: 0%;
      width: 1px;
      border-radius: 4px;
    }
    .line1 {
      @include flex(flex, row-reverse, center, center, 0rem);
      .arrow {
        height: 1px;
        width: 30px;
        background-color: red;
        border-radius: 4px;
      }
      .line {
        cursor: pointer;
        width: 400px;
        padding: 1.3rem 1.4rem;
        background-color: whitesmoke;
        border-radius: 18px;
        @include flex(flex, row, center, space-between, 0);
      }
    }
    .line {
      width: 400px;
      padding: 1.3rem 1.4rem;
      background-color: whitesmoke;
      border-radius: 18px;
      @include flex(flex, row, center, space-between, 0);
    }
  }
  .img-container {
    width: 40%;
    img {
      height: 80%;
      width: 60%;
    }
  }
  .btn {
    position: absolute;
    top: 2%;
    right: 14%;
    border: none;
    padding: 0.7rem 1.9rem;
    text-transform: capitalize;
    font-weight: 500;
    background-color: #c56376;
    color: #eee;
    border-radius: 10px;
  }
}
section > .part3 {
  padding: 4rem 10rem;
  min-height: 90vh;
  width: 100%;
  max-height: 100%;
  background: url("https://static.vecteezy.com/system/resources/previews/003/127/961/non_2x/abstract-template-background-white-and-gray-squares-free-vector.jpg");
  .card-container {
    // height: 70vh;
    // overflow: auto;
    @include flex(flex, row, center, space-between, 1rem);
    flex-wrap: wrap;
    .card {
      height: 250px;
      width: 350px;
      background-color: white;
      border-radius: 10px;
      padding: 0.8rem 0.9rem;
      .content {
        position: relative;
        @include flex(flex, row, center, space-between, 1rem);
      }
    }
  }
}
section > .part4 {
  padding: 6rem 10rem;
  @include flex(flex, column, center, center, 1rem);
  .list {
    @include flex(flex, row, center, space-between, 1rem);
    li {
      position: relative;
      @include flex(flex, column, center, center, 1rem);
      list-style: none;
      background-color: white;
      border-radius: 10px;
      height: 200px;
      width: 300px;
      .icon {
        position: absolute;
        bottom: 5%;
        right: 5%;
        opacity: 0.6;
      }
      &:hover {
        transition: all ease-in 0.3s;
        box-shadow: #c56376 0px 5px 15px;
        .icon {
          color: #c56376;
          opacity: 1;
        }
      }
    }
  }
}
.btn {
  position: absolute;
  top: 2%;
  right: 4%;
  border: none;
  padding: 0.7rem 1.9rem;
  text-transform: capitalize;
  font-weight: 500;
  background-color: #c56376;
  color: white;
  border-radius: 10px;
  cursor: pointer;
}
.user {
  // position: absolute;
  // top: 2%;
  // right: 4%;
  border: none;
  padding: 0.7rem 1.9rem;
  text-transform: capitalize;
  font-weight: 500;
  background-color: #c56376;
  color: white;
  border-radius: 10px;
  cursor: pointer;
}
.logo {
  height: 50px;
  width: 50px;
  border-radius: 50%;
  @include flex(flex, row, center, center);
  background-color: whitesmoke;
  i {
    color: $background-color;
  }
}
.footer {
  background-color: $background-color;
  color: white;
  padding: 4rem 10rem;
  @include flex(flex, row, center, space-between, 0);
  .first1 {
    @include flex(flex, column, flex-start, center, 0.4rem);
    .head {
      font-size: 24px;
      font-weight: 700;
      text-transform: capitalize;
    }
    li {
      list-style: none;
    }
    .links {
      margin-top: 0.6rem;
      @include flex(flex, row, flex-start, center, 0.9rem);
    }
  }
}
</style>
