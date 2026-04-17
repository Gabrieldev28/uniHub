<template>
<div class="login-container">
  
  <!-- FUNDO (shape) -->
  <div class="green-shape"></div>

  <!-- CONTEÚDO (logo + texto) -->
  <div class="left-content flex-col items-center w-2/4">
    <img src="../assets/logo.svg" class="logo" />
    <h3 class="text-3xl">Automatize. Organize. Converta.</h3>
  </div>

  <!-- LADO DIREITO (login) -->
  <div class="right-content w-2/4 bg-amber-900">
    <!-- form -->
     <h2 class="text-5xl">login</h2>
  </div>

</div>
</template>

<style>
.login-container {
  overflow: hidden;
}

/* SHAPE */
.green-shape {
  position: absolute;
  left: -30vw;
  width: 70vw;
  height: 110vh;

  background: #0b1d0b;

  border-radius: 200px;

  transform: rotate(-36deg);
  z-index: 1;
}

/* CONTEÚDO EM CIMA */
.left-content {
  position: absolute;
  left: 5%;
  top: 50%;
  transform: translateY(-50%);
  
  z-index: 2; /* 👈 MAIS IMPORTANTE */
}

</style>