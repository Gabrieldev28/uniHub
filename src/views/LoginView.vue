<template>
  <div class="relative w-full h-screen overflow-hidden">
    <!-- FUNDO (shape) -->
    <div class="green-shape shadow-2xl"></div>

    <!-- CONTEÚDO (logo + texto) -->
    <div class="relative z-2 w-full h-screen flex justify-around items-center">
      <div class="flex flex-col items-center justify-center w-2/6">
        <img src="../assets/logo.svg" class="max-w-72 gap-8" />
        <h3 class="text-2xl text-[#A6FF95]">Automatize. Organize. Converta.</h3>
      </div>

      <!-- LADO DIREITO (login) -->
      <div class="right-content w-2/6 text-[#111601] py-10 px-20">
        <!-- form -->
        <div>
          <h2 class="text-5xl font-semibold">LOGIN</h2>
          <p class="text-2xl">Bem vindo de volta!</p>
        </div>
        <div>
          <div class="p-3 flex gap-2 border-b border-[#111601]">
            <img src="../assets/icons/mail.svg" alt="mail" />
            <input
              type="text"
              placeholder="Email"
              class="placeholder:text-[#111601] placeholder:text-base w-full outline-none"
              name=""
              id=""
            />
          </div>
          <div>
            <div class="p-3 flex gap-2 border-b border-[#111601] justify-between">
              <div class="flex gap-2">
                <img src="../assets/icons/lock.svg" alt="lock" />
                <input type="password" placeholder="Senha" class="placeholder:text-[#111601] placeholder:text-base w-full outline-none" name="" id=""/>
              </div>
              <button><img src="../assets/icons/eye.svg" alt=""></button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
/* SHAPE */
.green-shape {
  position: absolute;
  left: -35vw;
  width: 80vw;
  height: 130vh;
  background: #111601;
  border-radius: 8rem;
  transform: rotate(-36deg);
  z-index: 1;
}

/* CONTEÚDO EM CIMA */
</style>