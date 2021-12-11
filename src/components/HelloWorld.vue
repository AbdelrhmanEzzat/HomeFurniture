<template>
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
                <MDBDropdownItem href="#">Something else here</MDBDropdownItem>
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
          <MDBNavbarItem to="#" class="me-2 me-lg-4"> Blog </MDBNavbarItem>
          <MDBNavbarItem to="#" class="me-2 me-lg-4"> Elements </MDBNavbarItem>
          <MDBNavbarItem to="#" class="me-2 me-lg-4"> Features </MDBNavbarItem>
        </MDBNavbarNav>
      </div>
    </MDBNavbarBrand>
  </MDBNavbar>
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
</style>
