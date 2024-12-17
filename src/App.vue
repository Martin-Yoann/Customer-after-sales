<template>
  <div id="app">
    <nav>
      <router-link to="/" class="menus">Home</router-link>
      <router-link to="/region" class="menus">REGION</router-link>
      <router-link to="/about" class="menus">ABOUT</router-link>
      <div class="menu">
        <img src="./assets/menu.png" class="menu-icon" />
      </div>
      <div class="title">
          <p>ClientNest</p>
      </div>
    </nav>
    <router-view/> 
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url(./assets/background.jpg);
  background-position: center;
  background-size: cover;
  padding-left: 8%;
  padding-right: 8%;
  box-sizing: border-box;
}
nav {
  padding: 30px;
  flex: 1;
  text-align: right;
  .title {
    position: absolute;
    left: 50%;
    top: 3%;
    transform: translateX(-50%);
    color: #fff;
    p{
      font-size: 20px;
      font-weight: 700;
    }
  }
  a {
    font-weight: bold;
    color: #fff;
    text-decoration: none;
    margin-left: 5vw;
    &.router-link-exact-active {
      color: #fff;
      box-shadow: 3px 5px 3px #ffffff00;
    }
  }
  ul li {
    list-style: none;
    display: inline-block;
    margin-left: 60px;
  }
  ul li a {
    text-decoration: none;
    color: #fff;
    font-size: 13px;
  }
}
.logo {
  width: 50px;
  cursor: pointer;
}
.menu{
  position: absolute;
  right: 0;
  top: 0;
  right: 5%;
  top: 2.3%;
}
.menu-icon {
  width: 30px;
  cursor: pointer;
  margin-left: 40px;
}

@media (max-width: 500px) {
  .menus{
    display: none;
  }
}
</style>
