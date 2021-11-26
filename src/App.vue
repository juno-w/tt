<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import QR from "./components/QR.vue";
</script>

<template>
  <section class="max-w-md mx-auto">
    <div>
      <img src="/images/header.png" alt="" />
    </div>

    <!-- Your COVID Health Status section -->
    <div class="px-4 font-medium text-gray-700">
      <div class="flex items-center justify-between py-4">
        <h3 class="font-semibold">Your COVID Health Status</h3>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          aria-hidden="true"
          role="img"
          class="w-5 h-5"
          preserveAspectRatio="xMidYMid meet"
          viewBox="0 0 24 24"
        >
          <path
            d="M19.33 6.694l.42-1.377a1 1 0 1 1 1.913.585l-1.17 3.825a1 1 0 0 1-1.248.664l-3.825-1.17a1 1 0 1 1 .585-1.912l1.672.511A7.381 7.381 0 0 0 4.685 9.084l-.26.633a1 1 0 1 1-1.85-.758l.26-.633A9.381 9.381 0 0 1 19.33 6.694zM3.808 17.307l-.327 1.311a1 1 0 1 1-1.94-.484l.967-3.88a1 1 0 0 1 1.265-.716l3.828.954a1 1 0 0 1-.484 1.941l-1.786-.445a7.384 7.384 0 0 0 13.216-1.792a1 1 0 1 1 1.906.608a9.381 9.381 0 0 1-5.38 5.831a9.386 9.386 0 0 1-11.265-3.328z"
            fill="currentColor"
          ></path>
        </svg>
      </div>

      <div>
        <div class="grid grid-cols-2 gap-4">
          <div class="rounded-md bg-[#eff9f9] p-2 text-center space-y-5">
            <p>Vaccinated</p>
            <div class="inline-block bg-white rounded-full">
              <svg class="w-10 h-10 text-[#208d85]" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                <path
                  fill-rule="evenodd"
                  d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                  clip-rule="evenodd"
                ></path>
              </svg>
            </div>
          </div>
          <div class="p-2 space-y-5 text-center bg-gray-200 rounded-md">
            <p>No test status</p>
            <div class="inline-block p-1 bg-white rounded-full shadow">
              <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" class="w-8 h-8 text-gray-200" viewBox="0 0 36 36">
                <path
                  d="M29.29 5H27v2h2v25H7V7h2V5H7a1.75 1.75 0 0 0-2 1.69v25.62A1.7 1.7 0 0 0 6.71 34h22.58A1.7 1.7 0 0 0 31 32.31V6.69A1.7 1.7 0 0 0 29.29 5z"
                  class="clr-i-outline clr-i-outline-path-1"
                  fill="currentColor"
                />
                <path
                  d="M26 7.33A2.34 2.34 0 0 0 23.67 5h-1.8a4 4 0 0 0-7.75 0h-1.79A2.34 2.34 0 0 0 10 7.33V11h16zM24 9H12V7.33a.33.33 0 0 1 .33-.33H16V6a2 2 0 0 1 4 0v1h3.67a.33.33 0 0 1 .33.33z"
                  class="clr-i-outline clr-i-outline-path-2"
                  fill="currentColor"
                />
                <path class="clr-i-outline clr-i-outline-path-3" d="M11 14h14v2H11z" fill="currentColor" />
                <path class="clr-i-outline clr-i-outline-path-4" d="M11 18h14v2H11z" fill="currentColor" />
                <path class="clr-i-outline clr-i-outline-path-5" d="M11 22h14v2H11z" fill="currentColor" />
                <path class="clr-i-outline clr-i-outline-path-6" d="M11 26h14v2H11z" fill="currentColor" />
              </svg>
            </div>
          </div>
        </div>
      </div>
    </div>

    <hr class="px-4 my-6 border-b border-gray-100" />

    <!-- SafeEntry check in section -->
    <div class="px-4">
      <div class="flex items-center justify-start py-2 space-x-2 font-medium text-gray-700">
        <img src="/images/se.png" alt="" class="w-8 h-8" />
        <h3 class="font-semibold">SafeEntry check in</h3>
      </div>
      <div class="bg-[#eaf4fd] py-4 rounded-md">
        <div class="grid grid-cols-3 place-items-center">
          <!-- scan qr -->
          <div class="text-center group hover:cursor-pointer">
            <div class="flex justify-center">
              <div class="inline-block p-1">
                <img src="/images/qr.png" alt="" class="w-16 h-16" />
              </div>
            </div>
            <p class="text-sm font-medium transition group-hover:text-blue-600">Scan QR</p>
          </div>
          <!-- Favourites -->
          <div class="text-center group hover:cursor-pointer">
            <div class="flex justify-center">
              <div class="inline-block p-1">
                <img src="/images/favourites.png" alt="" class="w-16 h-16" />
              </div>
            </div>
            <p class="text-sm font-medium transition group-hover:text-blue-600">Favourites</p>
          </div>
          <!-- Group -->
          <div class="text-center group hover:cursor-pointer">
            <div class="flex justify-center">
              <div class="inline-block p-1">
                <img src="/images/group.png" alt="" class="w-16 h-16" />
              </div>
            </div>
            <p class="text-sm font-medium transition group-hover:text-blue-600">Group</p>
          </div>
        </div>
      </div>
    </div>

    <hr class="my-6 border-b border-gray-100" />

    <!-- Stay safe together section -->
    <div class="px-4">
      <div
        class="flex items-center justify-between px-4 py-3 font-medium text-gray-700 border-2 border-dashed rounded-md  group hover:cursor-pointer"
      >
        <div class="h-14 w-14">
          <img src="/images/stay-safe-together.png" alt="" />
        </div>
        <div class="flex-1 px-4">
          <p>Stay safe together.</p>
          <p>Share the app!</p>
        </div>
        <div>
          <svg
            class="w-6 h-6 text-gray-500 group-hover:text-blue-600"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
              clip-rule="evenodd"
            ></path>
          </svg>
        </div>
      </div>
    </div>
  </section>
</template>

<style></style>
