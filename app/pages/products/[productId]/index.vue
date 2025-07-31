<template>
  <section class="w-full">
    <div class="w-full flex items-center justify-start">
      <ul class="app-container flex items-center justify-start gap-2.5 py-4">
        <li class="text-sm font-medium capitalize text-neutral-500">
          <nuxt-link :href="localePath('/')">home</nuxt-link>
        </li>
        <Icon name="tabler:chevron-right" />
        <li class="text-sm font-medium capitalize text-neutral-900">
          t-shirt brown xl size
        </li>
      </ul>
    </div>
    <!-- product images & infos wrapper -->
    <div
      class="app-container grid grid-cols-1 md:grid-cols-2 items-start justify-start gap-y-8 gap-x-32"
    >
      <!-- products images -->
      <div
        class="h-[574px] flex items-center justify-center rounded-md bg-neutral-white-100"
      >
        <swiper
          :slides-per-view="1"
          :space-between="20"
          :pagination="true"
          :modules="[Pagination]"
          @swiper="onSwiper"
          @slide-change="onSlideChange"
        >
          <swiper-slide>
            <nuxt-img
              src="https://picsum.photos/800/600"
              width="434"
              height="474"
            />
          </swiper-slide>
          <swiper-slide
            ><nuxt-img
              src="https://picsum.photos/801/600"
              width="434"
              height="474"
          /></swiper-slide>
          <swiper-slide
            ><nuxt-img
              src="https://picsum.photos/802/600"
              width="434"
              height="474"
          /></swiper-slide>
          ...
        </swiper>
      </div>
      <!-- product info -->
      <div>
        <span class="flex items-center justify-start gap-8 mb-3">
          <h3 class="text-2xl font-bold text-neutral-900 capitalize">
            t-shirt brown xl size
          </h3>
          <button
            type="button"
            class="flex items-center justify-center text-2xl"
          >
            <Icon name="mynaui:share" />
          </button>
        </span>
        <div class="flex items-center justify-start gap-2.5">
          <span
            class="flex items-center justify-center gap-1.5 bg-neutral-white-100 px-3 py-1 rounded-full text-neutral-500"
          >
            <Icon name="material-symbols-light:star-rounded" class="text-2xl" />
            <p class="text-xs font-medium">4.2 — 54 Reviews</p>
          </span>
          <span
            class="flex items-center justify-center gap-1.5 border border-neutral-white-100 px-3 py-1 rounded-full text-neutral-500"
          >
            <p class="text-xs font-medium">in stock</p>
          </span>
        </div>
        <h3 class="font-semibold text-lg capitalize text-neutral-900 mt-6">
          $ 150
        </h3>
        <div class="flex flex-col items-start justify-start gap-2.5 mt-8">
          <p class="uppercase font-medium text-xs text-neutral-500">
            Available Colors
          </p>
          <ul
            class="w-full md:max-w-fit grid grid-4 md:grid-cols-4 lg:grid-cols-5 items-start justify-start gap-2.5"
          >
            <li
              class="size-8 flex items-center justify-center p-0.5 border border-neutral-700 rounded-full"
            >
              <span class="size-full bg-amber-600 rounded-full" />
            </li>
            <li
              class="size-8 flex items-center justify-center p-0.5 border border-neutral-700 rounded-full"
            >
              <span class="size-full bg-emerald-600 rounded-full" />
            </li>
            <li
              class="size-8 flex items-center justify-center p-0.5 border border-neutral-700 rounded-full"
            >
              <span class="size-full bg-black rounded-full" />
            </li>
            <li
              class="size-8 flex items-center justify-center p-0.5 border border-neutral-700 rounded-full"
            >
              <span class="size-full bg-sky-600 rounded-full" />
            </li>
            <li
              class="size-8 flex items-center justify-center p-0.5 border border-neutral-700 rounded-full"
            >
              <span class="size-full bg-fuchsia-700 rounded-full" />
            </li>
            <li
              class="size-8 flex items-center justify-center p-0.5 border border-neutral-700 rounded-full"
            >
              <span class="size-full bg-indigo-700 rounded-full" />
            </li>
          </ul>
        </div>
        <div
          class="w-full md:max-w-1/3 flex items-start justify-start flex-col mt-4 gap-2.5"
        >
          <p class="uppercase font-medium text-xs text-neutral-500">
            Available Colors
          </p>
          <ul class="w-full grid grid-4 md:grid-cols-5 gap-2">
            <li
              class="size-10 flex items-center justify-center p-0.5 border border-neutral-900 rounded-md"
            >
              <label
                for="sm"
                class="size-full flex items-center justify-center cursor-pointer"
              >
                <input id="sm" type="text" hidden name="sm" />
                <p class="text-xs font-medium text-neutral-900 uppercase">sm</p>
              </label>
            </li>
            <li
              class="size-10 flex items-center justify-center p-0.5 border border-neutral-100 rounded-md"
            >
              <label
                for="lg"
                class="size-full flex items-center justify-center cursor-pointer"
              >
                <input id="lg" type="text" hidden name="lg" />
                <p class="text-xs font-medium text-neutral-900 uppercase">lg</p>
              </label>
            </li>
            <li
              class="size-10 flex items-center justify-center p-0.5 border border-neutral-100 rounded-md"
            >
              <label
                for="xl"
                class="size-full flex items-center justify-center cursor-pointer"
              >
                <input id="xl" type="text" hidden name="xl" />
                <p class="text-xs font-medium text-neutral-900 uppercase">xl</p>
              </label>
            </li>
            <li
              class="size-10 flex items-center justify-center p-0.5 border border-neutral-100 rounded-md"
            >
              <label
                for="2-xl"
                class="size-full flex items-center justify-center cursor-pointer"
              >
                <input id="2-xl" type="text" hidden name="2-xl" />
                <p class="text-xs font-medium text-neutral-900 uppercase">
                  2-xl
                </p>
              </label>
            </li>
            <li
              class="size-10 flex items-center justify-center p-0.5 border border-neutral-100 rounded-md"
            >
              <label
                for="3-xl"
                class="size-full flex items-center justify-center cursor-pointer"
              >
                <input id="3-xl" type="text" hidden name="3-xl" />
                <p class="text-xs font-medium text-neutral-900 uppercase">
                  3-xl
                </p>
              </label>
            </li>
          </ul>
        </div>
        <div class="flex flex-col items-start justify-start gap-2.5 mt-9">
          <p class="uppercase font-medium text-xs text-neutral-500">Quantity</p>
          <div
            class="flex items-center justify-center gap-7 px-2.5 py-1.5 border border-neutral-100 rounded-md"
          >
            <button
              type="button"
              class="p-2 text-neutral-500"
              :disabled="quantity === 0"
              @click="quantity = quantity - 1"
            >
              <Icon name="jam:minus" />
            </button>
            <h4 class="p-2 font-medium text-base">{{ quantity }}</h4>
            <button
              type="button"
              class="p-2 text-neutral-500"
              @click="quantity = quantity + 1"
            >
              <Icon name="jam:plus" />
            </button>
          </div>
        </div>
        <div class="flex items-center justify-start gap-4 mt-10">
          <button
            type="button"
            class="w-full md:w-[285px] rounded-md py-3 bg-neutral-900 text-neutral-100 hover:bg-neutral-800"
          >
            <p>add to cart</p>
          </button>
          <button
            type="button"
            class="w-fit flex items-center justify-center shrink-0 px-2 rounded-md py-2 border border-neutral-100 text-neutral-500"
          >
            <Icon name="lineicons:heart" class="text-3xl leading-3" />
          </button>
        </div>
      </div>
    </div>
    <!-- reviews and details -->
    <div class="app-container flex items-start justify-start gap-8 mt-44">
      <aside class="w-[240px] shrink-0 pt-20">
        <nav class="w-full grid-flow-row">
          <nuxt-link
            :href="{
              query: {
                menu: 'details',
              },
            }"
            class="w-full flex items-center justify-start mb-1.5 gap-2 hover:bg-neutral-white-100 text-neutral-900 px-3 py-2 rounded-md"
            :class="
              (route.query.menu === 'details' || !route.query.menu) &&
              'bg-neutral-white-100 pointer-events-none'
            "
          >
            <Icon name="pepicons-pencil:dots-x" class="text-2xl" />
            <p class="font-medium text-sm capitalize">details</p>
          </nuxt-link>
          <nuxt-link
            :href="{
              query: {
                menu: 'reviews',
              },
            }"
            class="w-full flex items-center justify-start mb-1.5 gap-2 hover:bg-neutral-white-100 text-neutral-900 px-3 py-2 rounded-md"
            :class="
              route.query.menu === 'reviews' &&
              'bg-neutral-white-100 pointer-events-none'
            "
          >
            <Icon name="stash:star-light" class="text-2xl" />
            <p class="font-medium text-sm capitalize">reviews</p>
          </nuxt-link>
        </nav>
      </aside>
      <div
        v-if="!route.query.menu || route.query.menu === 'details'"
        class="flex items-start justify-start gap-1 flex-col"
      >
        <h3 class="font-semibold text-base text-neutral-900 mb-6 capitalize">
          detail
        </h3>
        <p class="font-normal text-sm text-neutral-500">
          Elevate your everyday style with our Men's Black T-Shirts, the
          ultimate wardrobe essential for modern men. Crafted with meticulous
          attention to detail and designed for comfort, these versatile black
          tees are a must-have addition to your collection. The classic black
          color never goes out of style. Whether you're dressing up for a
          special occasion or keeping it casual, these black t-shirts are the
          perfect choice, effortlessly complementing any outfit.
        </p>
      </div>
      <div v-if="route.query.menu === 'reviews'" class="w-full flex flex-col">
        <h3 class="text-base font-semibold mb-4 text-neutral-900">Reviews</h3>
        <span class="flex items-center justify-start gap-3">
          <h3 class="font-bold text-4xl text-neutral-900">4.7</h3>
          <p class="text-sm text-neutral-400 font-normal">— 54 Reviews</p>
        </span>
        <!-- add reviews button -->
        <button
          type="button"
          class="w-fit py-3 px-6 border border-neutral-900 text-neutral-900 rounded-md mt-6 mb-14"
        >
          Write a review
        </button>
        <!-- reviews list -->
        <div
          class="w-full flex flex-col pt-16 border-t border-neutral-white-200"
        >
          <ul class="w-full grid grid-flow-row gap-3">
            <li class="w-full flex items-start justify-start gap-6 px-2 py-9">
              <figure
                class="size-12 flex items-center justify-center rounded-full shrink-0 font-semibold uppercase text-primary-900 bg-primary-100"
              >
                as
              </figure>
              <div class="flex-1">
                <h5
                  class="text-sm font-medium text-neutral-900 capitalize mb-1.5"
                >
                  Emily Davis
                </h5>
                <h6
                  class="text-xs font-medium text-neutral-500 capitalize mb-1.5"
                >
                  1 Week ago
                </h6>
                <p class="font-normal text-sm text-neutral-500 mt-4">
                  This company always goes above and beyond to satisfy their
                  customers.
                </p>
              </div>
              <div
                class="w-[140px] flex items-center justify-center gap-2 shrink-0"
              >
                <Icon name="ic:round-star" class="text-4xl text-neutral-900" />
                <Icon name="ic:round-star" class="text-4xl text-neutral-900" />
                <Icon name="ic:round-star" class="text-4xl text-neutral-900" />
                <Icon name="ic:round-star" class="text-3xl text-neutral-900" />
                <Icon name="iconamoon:star" class="text-3xl text-neutral-900" />
              </div>
            </li>
            <li class="w-full flex items-start justify-start gap-6 px-2 py-9">
              <figure
                class="size-12 flex items-center justify-center rounded-full shrink-0 font-semibold uppercase text-primary-900 bg-primary-100"
              >
                as
              </figure>
              <div class="flex-1">
                <h5
                  class="text-sm font-medium text-neutral-900 capitalize mb-1.5"
                >
                  Emily Davis
                </h5>
                <h6
                  class="text-xs font-medium text-neutral-500 capitalize mb-1.5"
                >
                  1 Week ago
                </h6>
                <p class="font-normal text-sm text-neutral-500 mt-4">
                  This company always goes above and beyond to satisfy their
                  customers.
                </p>
              </div>
              <div
                class="w-[140px] flex items-center justify-center gap-2 shrink-0"
              >
                <Icon name="ic:round-star" class="text-4xl text-neutral-900" />
                <Icon name="ic:round-star" class="text-4xl text-neutral-900" />
                <Icon name="ic:round-star" class="text-4xl text-neutral-900" />
                <Icon name="ic:round-star" class="text-3xl text-neutral-900" />
                <Icon name="iconamoon:star" class="text-3xl text-neutral-900" />
              </div>
            </li>
            <li class="w-full flex items-start justify-start gap-6 px-2 py-9">
              <figure
                class="size-12 flex items-center justify-center rounded-full shrink-0 font-semibold uppercase text-primary-900 bg-primary-100"
              >
                as
              </figure>
              <div class="flex-1">
                <h5
                  class="text-sm font-medium text-neutral-900 capitalize mb-1.5"
                >
                  Emily Davis
                </h5>
                <h6
                  class="text-xs font-medium text-neutral-500 capitalize mb-1.5"
                >
                  1 Week ago
                </h6>
                <p class="font-normal text-sm text-neutral-500 mt-4">
                  This company always goes above and beyond to satisfy their
                  customers.
                </p>
              </div>
              <div
                class="w-[140px] flex items-center justify-center gap-2 shrink-0"
              >
                <Icon name="ic:round-star" class="text-4xl text-neutral-900" />
                <Icon name="ic:round-star" class="text-4xl text-neutral-900" />
                <Icon name="ic:round-star" class="text-4xl text-neutral-900" />
                <Icon name="ic:round-star" class="text-3xl text-neutral-900" />
                <Icon name="iconamoon:star" class="text-3xl text-neutral-900" />
              </div>
            </li>
          </ul>
          <button
            type="button"
            class="text-neutral-900 border border-neutral-200 py-3 px-6 font-medium text-sm mt-16 rounded-md mx-auto"
          >
            Load more reviews
          </button>
        </div>
      </div>
    </div>
    <!-- Related Products -->
    <div class="app-container flex flex-col items-start justify-start mt-32">
      <h4 class="text-2xl font-bold mb-2">You might also like</h4>
      <p class="font-medium text-xs text-neutral-300 mb-14">SIMILAR PRODUCTS</p>
      <ul
        class="w-full grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 gap-x-6 gap-y-3"
      >
        <ProductsProductCard />
        <ProductsProductCard />
        <ProductsProductCard />
        <ProductsProductCard />
        <ProductsProductCard />
      </ul>
    </div>
    <!-- newsletter -->
    <HomeNewsletter class="mt-40" />
  </section>
</template>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Pagination } from "swiper/modules";
// Import Swiper styles
import "swiper/css";
import "swiper/css/pagination";

const quantity = shallowRef(1);
const route = useRoute();
const localePath = useLocalePath();
const onSwiper = (swiper) => {
  console.log(swiper);
};
const onSlideChange = () => {
  console.log("slide change");
};
useHeadSafe({
  titleTemplate: "e-commerce | t-shirt brown xl size",
});
</script>
<style lang="css">
.swiper {
  height: 100%;
  display: flex !important;
  align-items: center;
  justify-items: center;
}
.swiper-slide {
  display: flex !important;
  align-items: center;
  justify-items: center;
}
.swiper-slide > img {
  margin-inline: auto;
}
.swiper-pagination .swiper-pagination-bullet.swiper-pagination-bullet-active {
  background-color: var(--color-neutral-900);
}
.swiper-pagination .swiper-pagination-bullet {
  background-color: var(--color-neutral-500);
}
</style>
