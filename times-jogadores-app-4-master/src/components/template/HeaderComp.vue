<template>
  <header class="menu-superior">
    <div class="menu-esquerdo">
      <span> <RouterLink to="/">Home</RouterLink> </span>
      <span>|</span>
      <span> <RouterLink to="/jogadores">Jogadores</RouterLink> </span>
      <span>|</span>
      <span> <RouterLink to="/times">Times</RouterLink> </span>
    </div>
    <div class="menu-direito">
      <span> Sair</span>
    </div>
  </header>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Secular+One&display=swap');

header span {
  padding: 0 20px;
  font-family: 'Secular One', sans-serif;
}
.menu-superior {
  justify-content: space-between;
}
a{
  color: white;
}
</style>
