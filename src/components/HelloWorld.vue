<template>
  <header>
    <!-- Just an image -->
    <MDBNavbar light bg="light" container>
      <MDBNavbarBrand href="#">
        <img
          src="https://mdbootstrap.com/img/logo/mdb-transaprent-noshadows.png"
          height="40"
          alt=""
          loading="lazy"
        />
        <!---------------------- Icons ----------------------------->
        <div class="sticky-top">
          <MDBNavbarNav class="d-flex flex-row">
            <MDBNavbarItem to="#" class="me-3 me-lg-3">
              <MDBIcon icon="shopping-cart"></MDBIcon>
            </MDBNavbarItem>
            <MDBNavbarItem href="#" class="me-3 me-lg-3">
              <MDBIcon icon="heart" iconStyle="fas"></MDBIcon>
            </MDBNavbarItem>
            <!-- Icon dropdown -->
            <MDBNavbarItem class="me-3 me-lg-3 dropdown">
              <MDBDropdown v-model="dropdown3">
                <MDBDropdownToggle
                  tag="a"
                  class="nav-link"
                  @click="dropdown3 = !dropdown3"
                >
                  <MDBIcon icon="user" />
                </MDBDropdownToggle>
                <MDBDropdownMenu>
                  <MDBDropdownItem href="#">Action</MDBDropdownItem>
                  <MDBDropdownItem href="#">Another Action</MDBDropdownItem>
                  <MDBDropdownItem href="#"
                    >Something else here</MDBDropdownItem
                  >
                </MDBDropdownMenu>
              </MDBDropdown>
            </MDBNavbarItem>
          </MDBNavbarNav>
        </div>
        <!----------------------Section----------------------------->
        <div class="Section">
          <MDBNavbarNav class="d-flex flex-row">
            <MDBNavbarItem to="#" class="me-2 me-lg-3" active>
              Home
            </MDBNavbarItem>
            <MDBNavbarItem to="#" class="me-2 me-lg-4"> Sale </MDBNavbarItem>
            <MDBNavbarItem to="#" class="me-2 me-lg-4"> Pages </MDBNavbarItem>
            <MDBNavbarItem to="./About" class="me-2 me-lg-4">
              Blog
            </MDBNavbarItem>
            <MDBNavbarItem to="#" class="me-2 me-lg-4">
              Elements
            </MDBNavbarItem>
            <MDBNavbarItem to="#" class="me-2 me-lg-4">
              Features
            </MDBNavbarItem>
          </MDBNavbarNav>
        </div>
      </MDBNavbarBrand>
    </MDBNavbar>
    <!---------------------- Header ------------------------>
    <!-- Background image -->
    <div
      id="intro-example"
      class="p-5 text-center bg-image"
      alt="Wild Landscape"
      style="
        height: 500px;
        background-image: url('//cdn.shopify.com/s/files/1/0399/1126/0318/files/BossHomeLife-Home_1920x1200.jpg?v=1600330609');
      "
    >
      <div class="mask" style="background-color: rgba(0, 0, 0, 0.7)">
        <div class="d-flex justify-content-center align-items-center h-100">
          <div class="text-white">
            <h1 class="mb-3">Designed for Living</h1>
            <h5 class="mb-4">-</h5>
            <MDBBtn
              lg
              tag="a"
              outline="light"
              class="m-2"
              href="https://www.youtube.com/watch?v=c9B4TPnak1A"
              role="button"
              rel="nofollow"
              target="_blank"
              >Start tutorial</MDBBtn
            >
            <MDBBtn
              lg
              tag="a"
              outline="light"
              class="m-2"
              href="https://mdbootstrap.com/docs/b5/vue/"
              target="_blank"
              role="button"
              >Download MDB UI KIT</MDBBtn
            >
          </div>
        </div>
      </div>
    </div>
    <!-- Background image -->
  </header>
  <!-------------------------- Collection ---------------------------->
  <div class="Collection">
    <!-- Jumbotron -->
    <div class="p-5 text-center">
      <h4 class="intro-text">
        Boss atHome was created for the new ways we live and work. We make
        beautifully designed, sustainable furniture in the UK.
        <br />
        Human centric furniture, designed for living
      </h4>
      <a class="btn , link-dark" href="" role="button">Our Collection</a>
    </div>
    <!-- Jumbotron -->
  </div>
  <!------------------------- Gird ----------------------------->
  <MDBRow class="gird">
    <MDBCol md="4"
      ><div class="bg-image hover-overlay">
        <img
          src="https://cdn.shopify.com/s/files/1/0399/1126/0318/collections/hero_eafa3f87-3f78-4352-86ac-139dfef3512a_1920x1200.jpg?v=1596788896"
          class="img-fluid"
        />
        <a href="#!">
          <div
            class="mask overlay"
            style="background-color: rgba(57, 192, 237, 0.2)"
          ></div>
        </a></div
    ></MDBCol>
    <MDBCol md="4"
      ><div class="bg-image hover-overlay">
        <img
          src="https:/cdn.shopify.com/s/files/1/0399/1126/0318/collections/Boss_atHome_Product_-_Ola2_1920x1200.jpg?v=1596792348"
          class="img-fluid"
        />
        <a href="#!">
          <div
            class="mask overlay"
            style="background-color: rgba(57, 192, 237, 0.2)"
          ></div>
        </a></div
    ></MDBCol>
    <MDBCol md="4"
      ><div class="bg-image hover-overlay">
        <img
          src="https://cdn.shopify.com/s/files/1/0399/1126/0318/collections/Boss_atHome_Product_-_Bodie2_1920x1200.jpg?v=1596792894"
          class="img-fluid"
        />
        <a href="#!">
          <div
            class="mask overlay"
            style="background-color: rgba(57, 192, 237, 0.2)"
          ></div>
        </a></div
    ></MDBCol>
  </MDBRow>

  <div class="explore">
    <a class="btn , link-dark" href="" role="button">Explore Our Collection</a>
  </div>
  <!---------------------- Products ---------------------------->
  <MDBRow class="gird">
    <MDBCol col="2">col="6"</MDBCol>
    <MDBCol col="2">col="6"</MDBCol>
    <MDBCol col="2">col="6"</MDBCol>
    <MDBCol col="2">col="6"</MDBCol>
    <MDBCol col="2">col="6"</MDBCol>
    <MDBCol col="2">col="6"</MDBCol>
  </MDBRow>
</template>

<script>
import {
  MDBIcon,
  MDBNavbar,
  MDBNavbarNav,
  MDBNavbarBrand,
  MDBNavbarItem,
  MDBDropdown,
  MDBDropdownToggle,
  MDBDropdownMenu,
  MDBDropdownItem,
  MDBCol,
  MDBRow,
  MDBBtn,
} from "mdb-vue-ui-kit";
import { ref } from "vue";

export default {
  name: "HelloWorld",
  components: {
    MDBNavbarBrand,
    MDBIcon,
    MDBNavbar,
    MDBNavbarNav,
    MDBNavbarItem,
    MDBDropdown,
    MDBDropdownToggle,
    MDBDropdownMenu,
    MDBDropdownItem,
    MDBCol,
    MDBRow,
    MDBBtn,
  },
  setup() {
    const dropdown3 = ref(false);

    return {
      dropdown3,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.sticky-top {
  width: 10%;
  position: absolute;
  top: 8%;
  left: 90%;
  border-radius: 4px;
}

.Section {
  width: 40%;
  position: absolute;
  top: 15%;
  left: 50%;
  border-radius: 4px;
  font-size: smaller;
}
/**********************  Collection ************************/
.mb-3 {
  font-size: xxx-large;
}
.mb-4 {
  font-size: xxx-large;
}
.btn {
  font-family: grotesque-medium, sans-serif;
  margin-top: 1.5%;
}
.btn:hover {
  background-color: rgb(250, 250, 250);
}
.intro-text {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-style: normal;
  text-align: center;
  margin-top: revert;
  margin-bottom: revert;
  margin-left: 15%;
  margin-right: 15%;
  line-height: 1.5;
}
/************************** Gird *****************************/
.gird {
  width: 100%;
  position: relative;
  margin: 10px 0 10px;
  padding-left: 2%;
  padding-right: 2%;
  padding-top: 6%;
  padding-bottom: 5%;
  text-align: center;
}
.col-md-4 {
  padding: 0px 30px;
}
.explore {
  padding-left: 42%;
  /* padding-bottom: 10%; */
}
</style>
