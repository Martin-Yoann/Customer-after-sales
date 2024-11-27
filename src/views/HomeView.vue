<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <h2>Strategic, purpose-driven business service crafted for your success.</h2>
        <p>
          As we are committed to delivering unparalleled service and exceptional results, guided by our extensive
          experience and expertise.
        </p>
        <button type="button">Explore</button>
      </div>
      <div class="col">
        <div class="card1 card">
          <!-- <h5>Western Desert</h5>
          <p>no other member state of the United Nations had ever officially recognized</p> -->
        </div>
        <div class="card2 card">
          <!-- <h5>AI Bagawat</h5>
          <p>no other member state of the United Nations had ever officially recognized</p> -->
        </div>
        <div class="card3 card">
          <!-- <h5>Pyramid of Giza</h5>
          <p>no other member state of the United Nations had ever officially recognized</p> -->
        </div>
        <div class="card4 card">
          <!-- <h5>Kalahari Desert</h5>
          <p>no other member state of the United Nations had ever officially recognized</p> -->
        </div>

      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'HomeView',
  components: {
    
  }
}
</script>
<style>
* {
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
}

.row {
  display: flex;
  height: 88%;
  align-items: center;
  margin-top: 10%;
}

.col {
  flex-basis: 50%;
}

h2 {
  color: #fff;
  font-size: 1.5rem;
}

p {
  color: #fff;
  font-size: 11px;
  line-height: 15px;
}

button {
  width: 180px;
  color: #000;
  font-size: 12px;
  padding: 12px 0;
  background: #fff;
  border: 0;
  border-radius: 20px;
  outline: none;
  margin-top: 30px;
  cursor: pointer;
}

.card {
  width: 240px;
  height: 230px;
  display: inline-block;
  border-radius: 10px;
  padding: 15px 25px;
  box-sizing: border-box;
  cursor: pointer;
  margin: 10px 15px;
  background-position: center;
  background-size: cover;
  transition: transform 0.5s;
}

.card1 {
  background-image: url(../assets/banner.jpg);
}

.card2 {
  background-image: url(../assets/banner2.jpg);
}

.card3 {
  background-image: url(../assets/banner1.jpg);
}

.card4 {
  background-image: url(../assets/banner3.jpg);
}

.card:hover {
  transform: translateY(-10px);
}

h5 {
  color: #fff;
  text-shadow: 0 0 5px #999;
}

.card p {
  text-shadow: 0 0 5px #000;
  font-size: 8px;
}

@media (max-width: 900px) {
  .card {
    display: none;
  }
  .row{
    width: 100%;
    display: block;
    margin-top: 65%;
  }

  .col {
    width: 100%;
  }

  .col h2 {
    width: 100%;
  }
  .col p{
    margin-top: 5%;
  }
}
</style>
