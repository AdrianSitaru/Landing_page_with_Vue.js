<template>
  <div class="Navbar">
    <img class="HeaderLogo" src="../assets/spotify_logo2.jpg" alt="image" />
    <span class="HamburgerMenu">|||</span>
    <ul class="NavbarContent">
      <li>
        <a href="#">Premium</a>
      </li>
      <li>
        <a href="#">Asistență</a>
      </li>
      <li>
        <a href="#">Descarcă</a>
      </li>
      <li>
        <span id="headerSign">|</span>
      </li>
      <li>
        <a href="#">Înregistrează-te</a>
      </li>
      <li>
        <a href="#">Conectează-te</a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "TheHeader",
};
</script>
<style scoped>
.HeaderLogo {
  height: 45px;
  width: 125px;
  margin-top: 5px;
  margin-left: 15px;
  cursor: pointer;
}

.Navbar {
  background-color: black;
  display: flex;
  justify-content: space-between;
}

.HamburgerMenu {
  color: white;
  transform: rotate(90deg);
}

.NavbarContent {
  margin-top: 10px;
  display: flex;
  justify-content: space-between;
  list-style: none;
  color: white;
}

.NavbarContent li a {
  color: white;
  text-decoration: none;
  padding: 20px;
  margin-top: 20px;
}

@media (min-width: 992px) {
  .Navbar .HamburgerMenu {
    display: none;
  }
}
</style>
