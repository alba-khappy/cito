<template>

  <header class="header">
      <img src="../assets/logo.svg" alt="Министерство науки и высшего образования Российской Федерации">
      <a href="" class="header__profile">
        <p>{{Иванов}} {{Иван}}</p>
        <img src="../assets/profile.png" alt="Фото профиля" class="header__profile-photo">
      </a>
      
    </header>
    
</template>

<style scoped>

.header {
  display: grid;
  grid-template-columns: auto 1fr;
  align-items: center;
}

.header__profile {
  display: grid;
  grid-template-columns: repeat(3, auto);
  justify-content: right;
  align-items: center;
  column-gap: 10px;
}

.header__profile::after {
  content: '';
  background-image: url("../assets/arrow.svg");
  background-repeat: no-repeat;
  width: 12px;
  height: 6px;
}


</style>