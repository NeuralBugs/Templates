<template>
    <v-app id="inspire">
    <v-app-bar color="white" app fixed class="d-flex justify-space-around">
      <v-img
        max-width="111"
        src="../assets/newneuralrmbg.png"
        class="align-start"
      ></v-img>

      <v-app-bar-items class="hidden-xs-only color ml-16">
        <v-btn text><router-link to="/">Home</router-link></v-btn>

        <v-btn text
          ><router-link to="/About">Education</router-link></v-btn
        >
        <v-btn text
          ><router-link to="/Services">Services</router-link></v-btn
        >
        <v-btn text><router-link to="/Contacts">Contact us</router-link></v-btn>
      </v-app-bar-items>
      <div class="hidden-sm-and-up">
        <v-menu offset-y>
          <template v-slot:activator="{ on }">
            <v-app-bar-nav-icon v-on="on"></v-app-bar-nav-icon>
          </template>
          <v-list class="responsiveMenu color">
            <v-list-item>
              <v-list-item-title
                ><router-link to="/">Home</router-link></v-list-item-title
              >
            </v-list-item>
            <v-list-item>
              <v-list-item-title
                ><router-link to="/Services"
                  >Education</router-link
                ></v-list-item-title
              >
            </v-list-item>
            <v-list-item>
              <v-list-item-title
                ><router-link to="/About"
                  > Services
                </router-link></v-list-item-title
              >
            </v-list-item>
            <v-list-item>
              <v-list-item-title
                ><router-link to="/Contacts"
                  >Contact us</router-link
                ></v-list-item-title
              >
            </v-list-item>
          </v-list>
        </v-menu>
      </div>
      <div class="icon">
               <div class="navtitle">
          <h2 class="text-h4 font-weight-black">
          </h2>
        </div>
        <div class="navlog .d-flex justify-end">
          <v-btn icon class="mr-2">
            <i class="fa-brands fa-instagram"></i>
          </v-btn>

          <v-btn icon class="mr-2">
            <i class="fa-brands fa-facebook"></i>
          </v-btn>
          <v-btn icon class="mr-2"><i class="fa-brands fa-twitter"></i></v-btn>
          </div>
        </div>
    </v-app-bar>
  </v-app>
</template>

<script>
export default {
  name: "Header-index",
  data: () => ({}),
};
</script>

<style lang="scss" scoped>
span {
  a {
    color: black;
  }
}
.router-link-active{
  color: black;
}

   a{
      text-decoration: none;
      color: black;   
    }
    i {
      color: black;
      font-size: 12px;
    }
@media screen and (min-width: 80rem) {
  .container {
    width: 100%;
    a{
      text-decoration: none;
    }
  }
}
.tou {
  box-shadow: 0px 3px 1px -2px rgb(0 0 0 / 20%),
    0px 2px 2px 0px rgb(0 0 0 / 14%), 0px 1px 5px 0px rgb(0 0 0 / 12%) !important;
    .flex{
      display: flex;
      align-items: center;
      a{
        text-decoration: none;
        display: none;
      }
    }
  .menutab {
    max-width: 890px;
    margin-right: auto;
    margin-left: auto;
    text-align: center;
    color: black;
    a {
      text-decoration: none;
      color: black;
    }
    i {
      margin-left: 8px;
      color: black;
      font-size: 17px;
    }
  }
}
.navb {
  padding: 20px;
  .navtitle {
    h2 {
      text-transform: uppercase;
    }
  }
  display: flex;
  align-items: center;
  justify-content: space-around;
  .navlog {
    i {
      color: red;
      font-size: 25px;
    }
  }
}
</style>
