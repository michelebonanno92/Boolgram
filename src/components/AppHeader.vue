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
      <img src="/public/logo.png" alt="logo">
    </div>
    <div>
      <button class="button-header">Cerca</button>
    </div>
    <div>

    </div>

  </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

header{
  display: flex;
  justify-content: space-between;
  align-items: center;
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

</style>
