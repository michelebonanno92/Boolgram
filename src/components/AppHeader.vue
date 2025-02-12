<script>
export default {
  data() {
    return { 
     
    }
  }
}
</script>

<template>
  <header>
    <div>
     <a href="#">
       <img src="/public/logo.png" alt="logo">
     </a>
      
    </div>
    <div>
      <button class="button-header">Cerca</button>
    </div>
    <div class="header-right">
      <a href="#">
        <i class="fa-regular fa-heart"></i>
      </a>
      <a href="#">
        <i class="fa-solid fa-house"></i>
      </a>
      <a href="#" class="profile-circle">
        <img src="/public/profile.jpg" alt="Foto profilo">
      </a>
    </div>

  </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

header{
  max-width: 1200px;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}
header img{
  max-width: 100px;
}
.button-header{
  padding: 0 80px;
  background-color: white;
  border: 2px solid #d3d3d3;
  color: gray;
  // transition: border-color 0.3s ease;
}
.button-header:hover{
  border-color: #b0b0b0;
  color: black;  
}

.fa-heart {
  font-size: 24px;  /* Dimensione */
  color: black;     /* Colore del bordo */
  cursor: pointer;
}
.fa-house {
  font-size: 24px;  /* Dimensione */
  color: black;     /* Colore nero */
}

.profile-circle {
  width: 50px;                /* Larghezza del cerchio */
  height: 50px;               /* Altezza del cerchio */
  border-radius: 50%;          /* Trasforma in cerchio */
  overflow: hidden;            /* Taglia i contenuti in eccesso */
  display: flex;               /* Allinea il contenuto (immagine) */
  justify-content: center;
  align-items: center;
  background: linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888); /* Gradiente Instagram */
  padding: 2px;                /* Spazio interno per il bordo gradiente */
}

.profile-circle img {
  width: 100%;                 /* L'immagine riempie il cerchio */
  height: 100%;                /* Mantiene proporzioni */
  object-fit: cover;           /* Taglia l'immagine per adattarla al cerchio */
  border-radius: 50%;          /* Arrotonda l'immagine per seguire il cerchio */
}

.header-right{
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header-right > a{
  margin-right: 20px;
}





</style>
