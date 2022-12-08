<template>
  <div class="container">
    <div class="judul">
      <h1>Pilihan Karir Kamu</h1>
    </div>

    <div class="cardContainer">
      <div class="card">
        <div class="picture">
          <img src="../assets/image/front end.png" />
          <p>Front End</p>
        </div>
        <div class="icons">
          <a href=""
            ><font-awesome-icon icon="fa-solid fa-chevron-right fa-2xl"
          /></a>
        </div>
      </div>

      <div class="card">
        <div class="picture">
          <img src="../assets/image/backend.png" />
          <p>Back End</p>
        </div>
        <div class="icons">
          <a href=""
            ><font-awesome-icon icon="fa-solid fa-chevron-right fa-2xl"
          /></a>
        </div>
      </div>

      <div class="card">
        <div class="picture">
          <img src="../assets/image/backend.png" />
          <p>Back End</p>
        </div>
        <div class="icons">
          <a href=""
            ><font-awesome-icon icon="fa-solid fa-chevron-right fa-2xl"
          /></a>
        </div>
      </div>

      <div class="card">
        <div class="picture">
          <img src="../assets/image/backend.png" />
          <p>Back End</p>
        </div>
        <div class="icons">
          <a href=""
            ><font-awesome-icon icon="fa-solid fa-chevron-right fa-2xl"
          /></a>
        </div>
      </div>

      <div class="card">
        <div class="picture">
          <img src="../assets/image/backend.png" />
          <p>Back End</p>
        </div>
        <div class="icons">
          <a href=""
            ><font-awesome-icon icon="fa-solid fa-chevron-right fa-2xl"
          /></a>
        </div>
      </div>

      <div class="card">
        <div class="picture">
          <img src="../assets/image/backend.png" />
          <p>Back End</p>
        </div>
        <div class="icons">
          <a href=""
            ><font-awesome-icon icon="fa-solid fa-chevron-right fa-2xl"
          /></a>
        </div>
      </div>
    </div>

    <div class="collaps">
      <button>Lihat Semua</button>
    </div>

    <figure v-for="card in cards">
      <figcaption>{{ card.judul }}</figcaption>
      <img src="{{ card.image }}" />
    </figure>
  </div>
</template>

<script setup>
const cards = [
  { judul: "Front End", images: "../../assets/image/backend.png" },
];
</script>

<style scoped>
.container {
  margin-left: 76px;
  margin-right: 76px;
  margin-top: 50px;
}

.judul {
  font-weight: 700;
  text-align: center;
  align-items: center;
  padding-bottom: 106px;
}

.cardContainer {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
  gap: 30px;
}
.card {
  max-width: 22rem;
  height: 170px;
  border-radius: 15px;
  display: flex;
  align-items: center;
  background-color: #dddd;
  gap: 160px;
  padding-left: 35px;
  padding-right: 20px;
}
.picture img {
  height: 100px;
  max-width: 150px;
  border-radius: 5px;
}

.picture p {
  font-weight: 700;
  font-size: 25px;
  padding-top: 5px;
}

.icons {
  background-color: #4a7aba;
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 100%;
}

.icons a {
  color: #ffffff;
  background-color: #4a7aba;
}

.collaps {
  display: flex;
  justify-content: center;
  padding-top: 40px;
  padding-bottom: 40px;
}
.collaps button {
  background-color: #232e35;
  color: #ffffff;
  width: 210px;
  height: 55px;
  border-radius: 5px;
  border: none;
  font-size: 18px;
  font-weight: 600;
  cursor: pointer;
}
</style>
