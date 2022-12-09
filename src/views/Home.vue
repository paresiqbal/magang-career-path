<template>
  <div class="container">
    <div class="judul">
      <h1>Pilihan Karir Kamu</h1>
    </div>

    <div class="cardContainer">
      <div class="card" v-for="card in cards" :key="card.key">
        <div class="picture">
          <img :src="card.images" alt="backend.png" />
          <p>{{ card.judul }}</p>
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

    <!-- <figure v-for="card in cards" :key="card.key">
      <p>{{ card.judul }}</p>
      <img :src="card.images" alt="backend.png" />
    </figure> -->
  </div>
</template>

<script setup>
import { ref } from "vue";

const cards = ref([
  { key: 1, judul: "Frontend", images: "src/assets/image/frontend.png" },
  {
    key: 2,
    judul: "Backend",
    images: "src/assets/image/backend.png",
  },
  {
    key: 3,
    judul: "UI/UX",
    images: "src/assets/image/uiux.png",
  },
  {
    key: 4,
    judul: "Product Manager",
    images: "src/assets/image/produkmanager.png",
  },
  {
    key: 5,
    judul: "System Analist",
    images: "src/assets/image/systemanalis.png",
  },
  {
    key: 6,
    judul: "Quality Asurance",
    images: "src/assets/image/qualityasurance.png",
  },
  {
    key: 7,
    judul: "Digital Marketing",
    images: "src/assets/image/digitalmarketing.png",
  },
  {
    key: 8,
    judul: "Business Development",
    images: "src/assets/image/businesdevelopment.png",
  },
  {
    key: 9,
    judul: "Content Creator",
    images: "src/assets/image/contentcreator.png",
  },
  {
    key: 10,
    judul: "Graphic Design",
    images: "src/assets/image/graphicdesign.png",
  },
  {
    key: 11,
    judul: "3D",
    images: "src/assets/image/3dmodeling.png",
  },
]);
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
  /* max-width: 22rem; */
  height: 170px;
  border-radius: 15px;
  display: flex;
  align-items: center;
  background-color: #dddd;
  padding-left: 35px;
  padding-right: 20px;
}

.picture {
  width: 260px;
}
.picture img {
  max-width: 150px;
  height: 90px;
  border-radius: 5px;
}

.picture p {
  font-weight: 700;
  font-size: 22px;
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
