<template>
  <div class="relative w-full h-screen overflow-hidden">
    <!-- FUNDO (shape) -->
    <div class="green-shape shadow-2xl"></div>

    <!-- CONTEÚDO (logo + texto) -->
    <div class="relative z-2 w-full h-screen flex justify-around items-center">
      <div class="flex flex-col items-center justify-center w-2/6 gap-2">
        <img src="../assets/logo.svg" class="max-w-72 w-5/8" />
        <h3 class="text-2xl text-[#A6FF95]">Automatize. Organize. Converta.</h3>
      </div>

      <!-- LADO DIREITO (login) -->
      <div class="right-content w-2/6 flex flex-col text-[#111601] py-10 px-20 max-w-140 gap-8">
        <!-- form -->
        <div class="flex flex-col">
          <h2 class="text-2xl font-semibold">LOGIN</h2>
          <p class="text-lg">Bem vindo de volta!</p>
        </div>
        <!-- input part-->
        <div class="flex flex-col gap-2">
          <div class="p-2 flex gap-2 border-b border-[#111601]">
            <img src="../assets/icons/mail.svg" alt="mail" />
            <input
              type="text"
              placeholder="Email"
              class="placeholder:text-[#111601] placeholder:text-sm w-full outline-none"
              name=""
              id=""
            />
          </div>

          <div>
            <div class="p-2 flex gap-2 border-b border-[#111601] justify-between">
              <div class="flex gap-2">
                <img src="../assets/icons/lock.svg" alt="lock" />
                <input
                  :type="showPassword ? 'text' : 'password'"
                  placeholder="Senha"
                  class="placeholder:text-[#111601] placeholder:text-sm w-full outline-none"
                />
              </div>

              <button type="button" @click="showPassword = !showPassword">
                <img :src="showPassword ? eyeOff : eye" />
              </button>
            </div>
            <div class="flex gap-2 my-2">
              <input type="checkbox" />
              <p class="text-xs">Lembrar minha senha</p>
            </div>
          </div>
        </div>

        <div class="flex flex-col gap-4">
          <button
            class="w-full p-4 rounded-lg bg-[#111601] text-white hover:bg-[#A6FF95] hover:text-black hover:font-semibold hover:scale-105 text-sm"
          >
            Entrar
          </button>
          <a href="" class="text-center font-semibold text-sm">Esqueci minha senha</a>
        </div>
        <div class="flex flex-col text-center gap-1">
          <div class="flex flex-col text-sm">
            <p>Não tem Acesso?</p>
            <p>Para criar sua conta em poucos passos</p>
          </div>
          <a href="" class="font-semibold text-sm">Clique Aqui!</a>
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
  border-radius: 10rem;
  transform: rotate(-40deg);
  z-index: 1;
}

/* CONTEÚDO EM CIMA */
</style>

<script setup>
import { ref } from 'vue'

import eye from '../assets/icons/eye.svg'
import eyeOff from '../assets/icons/eye-close.svg'

const showPassword = ref(false)
</script>