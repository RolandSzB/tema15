<script setup>
import MainProduct from "./components/MainProduct.vue";
import "bootstrap-icons/font/bootstrap-icons.css";

const products = [
  {
    icon: "bi bi-twitch text-purple-700",
    name: "Twitch Posts",
    newValue: "500.00",
    unit: "$",
    value: "+40.5% ",
    valueColor: "text-green-500",
    moving: "more impressions",
    info: "0.5% MRR",
  },
  {
    icon: "bi bi-twitter text-blue-500",
    name: "Twitter Folloers",
    newValue: "807",
    unit: "k",
    value: "+17.62% ",
    valueColor: "text-green-500",
    moving: "Followers Growth",
    info: "5% New trials",
  },
  {
    icon: "bi bi-spotify text-green-500",
    name: "Spotify Listeners",
    newValue: "1,073",
    unit: "",
    value: "+10.45% ",
    valueColor: "text-red-500",
    moving: " Less comments than usual",
    info: "40% Impressions",
  },
  {
    icon: "bi bi-pinterest text-red-500",
    name: "Pinterest Posts",
    newValue: "97",
    unit: "",
    value: "+26.1% ",
    valueColor: "text-green-500",
    moving: "More posts",
    info: "10% Spend",
  },
  {
    icon: "bi bi-github text-purple-500",
    name: "Github Contributes",
    newValue: "4,109",
    unit: "",
    value: "+32.8% ",
    valueColor: "text-red-500",
    moving: " Less contributions",
    info: "40% Dispute",
  },
  {
    icon: "bi bi-youtube text-red-500",
    name: "Youtube Subscribers",
    newValue: "354",
    unit: "",
    value: "+29.45% ",
    valueColor: "text-green-500",
    moving: "Subscribers Growth",
    info: "40% Subscribers",
  },
];
</script>

<template>
  <div class="flex flex-row ms-5">
    <MainProduct v-for="product in products" :details="product" />
  </div>
</template>

<style>
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>
