<script setup>
import { TeamCard } from "@/components";
import { team } from "@/data";
import "swiper/css";
import "swiper/css/pagination";
import { Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
</script>

<template>
  <section
    class="container flex flex-auto flex-col items-center justify-center"
  >
    <h3 class="text-center text-3xl font-bold" @click="onSlideChange">
      Tim<span class="ml-1 text-yellow-600">WEBGIS.</span>
    </h3>
    <swiper
      class="my-16 w-full"
      :slidesPerView="1"
      :breakpoints="{
        768: {
          slidesPerView: 3,
        },
        1024: {
          slidesPerView: 4,
        },
      }"
      :loop="true"
      :autoplay="true"
      :pagination="{
        dynamicBullets: true,
        clickable: true,
        dynamicMainBullets: 3,
      }"
      :modules="[Pagination]"
    >
      <swiper-slide v-for="member in team">
        <team-card
          :key="member.id"
          :name="member.name"
          :role="member.role"
          :image="member.image"
          :link="member.link"
        />
      </swiper-slide>
    </swiper>
  </section>
</template>
