<template>
  <div class="bcg">
    <div class="bg">
      <div class="showcase">
        <div class="video-container">
          <video src="../assets/background.mp4" autoplay muted loop></video>
        </div>
        <div class="content">
          <h1 class="h11">Bem-vindos</h1>
          <h2 class="h22">
            Embaixada da República de Angola na República Federal da Alemanha
          </h2>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import HomeView from "../views/HomeView.vue";
export default {
  // components: { HomeView },
  name: " Background-index",
  //   data() {
  //     return {
  //       user: "Background",
  //     };
  //   },
};
</script>
<style lang="scss">
.h11 {
  font-weight: 500;
  // font-size: 75px;
  line-height: 1.2;
  margin-bottom: 15px;
  text-transform: uppercase;
}
.h22 {
  // font-size: 50px;
  line-height: 1.2;
  font-weight: 500;
  text-transform: uppercases;
}
.showcase {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: #fff;
  padding: 0 20px;
}

.video-container {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
  background: var(--primary-color) url("../assets/background.mp4") no-repeat
    center center/cover;
}

.video-container video {
  min-width: 100%;
  min-height: 83%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  object-fit: cover;
}

.video-container:after {
  content: "";
  z-index: 1;
  height: 100%;
  width: 100%;
  top: 0;
  left: 0;
  // background: rgba(0, 0, 0, 0.5);
  position: absolute;
}

.content {
  z-index: 2;
}

// .btn {
//   display: inline-block;
//   padding: 10px 30px;
//   background: var(--primary-color);
//   color: #fff;
//   border-radius: 5px;
//   border: solid #fff 1px;
//   margin-top: 25px;
//   opacity: 0.7;
// }

// .btn:hover {
//   transform: scale(0.98);
// }

.about {
  padding: 40px;
  text-align: center;
  p {
    font-size: 1.2rem;
    max-width: 600px;
    margin: auto;
  }
  h2 {
    margin: 30px 0;
    color: var(--primary-color);
  }
  a {
    margin: 0 5px;
  }
}
</style>
