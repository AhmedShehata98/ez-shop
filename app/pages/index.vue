<template>
  <section class="w-full min-h-screen flex flex-col">
    <!-- offers banners -->
    <div class="w-full min-h-[440px] bg-neutral-white-100 py-6 md:py-0">
      <!-- banner item -->
      <div
        class="app-container h-full flex flex-col md:flex-row gap-y-20 items-center justify-between"
      >
        <span>
          <h4
            class="text-neutral-800 text-start font-semibold text-4xl capitalize"
          >
            {{ $t("index.banner.fresh_arrivals") }}
          </h4>
          <p class="text-neutral-600 text-start font-normal text-sm">
            {{ $t("index.banner.discover_collection") }}
          </p>
          <button
            type="button"
            class="flex items-center justify-center gap-3 px-3 py-2 rounded-md text-white bg-neutral-900 mt-5"
          >
            <p class="text-inherit">{{ $t("index.banner.view_collection") }}</p>
            <Icon name="si:arrow-right-duotone" class="text-inherit text-2xl" />
          </button>
        </span>
        <span class="relative place-self-end">
          <svg
            width="340"
            height="340"
            viewBox="0 0 340 340"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <circle opacity="0.6" cx="170" cy="170" r="170" fill="#E9E9EB" />
            <path
              d="M46 21.9689C38.5464 22.6339 34.2639 23.2457 31.6348 25.2674C28.5449 27.6349 27.8131 31.9709 27 40.6429C26.1598 31.6517 25.4009 27.3423 22.0128 25.028C19.3837 23.2191 15.1284 22.6339 8 21.9955C15.4265 21.3304 19.7361 20.7186 22.3381 18.7235C25.4551 16.3294 26.1869 12.02 27 3.32144C27.7589 11.3284 28.4365 15.6112 30.9572 18.0851C33.4779 20.559 37.8688 21.2506 46 21.9689Z"
              fill="#E6E7E8"
            />
          </svg>
          <nuxt-img
            src="/images/e52f9cf6cc856def87647021dd851ac0c535f64b.png"
            alt="e52f9cf6cc856def87647021dd851ac0c535f64b.png"
            width="255"
            height="380"
            class="absolute bottom-0 left-1/2 -translate-x-1/3"
          />
        </span>
      </div>
    </div>
    <!-- features -->
    <div class="app-container mt-20 mb-32">
      <ul class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 md:gap-8">
        <li v-for="item in FEATURES_LIST" :key="item.title">
          <span
            class="size-12 flex items-center justify-center rounded-full mb-6 bg-neutral-white-100 text-2xl"
          >
            <Icon :name="item.icon" />
          </span>
          <h5 class="font-semibold text-base text-neutral-800">
            {{ item.title }}
          </h5>
          <p class="font-normal text-sm text-neutral-500">
            {{ item.description }}
          </p>
        </li>
      </ul>
    </div>
    <!-- best selling -->
    <div class="w-full flex flex-col items-center justify-center gap-20 mb-40">
      <span class="w-full flex flex-col items-center justify-center gap-2.5">
        <p
          class="font-medium text-xs text-neutral-300 justify-self-start text-start"
        >
          {{ $t("index.products.shop_now") }}
        </p>
        <h3 class="text-neutral-900 text-start font-bold text-2xl">
          {{ $t("index.products.best_selling") }}
        </h3>
      </span>
      <ul
        class="app-container grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-5"
      >
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
      </ul>
    </div>
    <!-- banner -->
    <div
      class="w-full min-h-[300px] flex items-center justify-center bg-neutral-white-100"
    >
      <div
        class="app-container flex flex-col md:flex-row items-center justify-between gap-y-6 py-6 md:py-0"
      >
        <span>
          <h4
            class="text-neutral-800 text-start font-semibold text-4xl capitalize"
          >
            {{ $t("index.banner.browse_fashion") }}
          </h4>
          <p class="text-neutral-600 text-start font-normal text-sm">
            {{ $t("index.banner.explore_collection") }}
          </p>
          <button
            type="button"
            class="flex items-center justify-center gap-3 px-3 py-2 rounded-md text-white bg-neutral-900 mt-5"
          >
            <p class="text-inherit">{{ $t("index.banner.start_browsing") }}</p>
            <Icon name="si:arrow-right-duotone" class="text-inherit text-2xl" />
          </button>
        </span>
        <nuxt-img
          src="/images/8cc9f607e22ea11cc9c0fb0df83525da3489524f.png"
          alt="8cc9f607e22ea11cc9c0fb0df83525da3489524f.png"
          width="225"
          height="311"
        />
      </div>
    </div>
    <!-- filtered products -->
    <div
      class="app-container flex flex-col items-center justify-center mt-36 mb-40 gap-16"
    >
      <ul class="flex items-center justify-center gap-5">
        <!-- active btn -->
        <li>
          <button
            type="button"
            class="flex items-center justify-center px-3 py-2 rounded-full border border-neutral-white-200 text-sm text-neutral-800 font-medium capitalize"
          >
            {{ $t("index.products.featured") }}
          </button>
        </li>
        <!-- non-active btn -->
        <li>
          <button
            type="button"
            class="flex items-center justify-center px-3 py-2 rounded-full text-sm text-neutral-500 font-normal capitalize"
          >
            {{ $t("index.products.latest") }}
          </button>
        </li>
      </ul>
      <ul class="w-full grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-9">
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
      </ul>
    </div>
    <!-- newsletter -->
    <div
      class="w-full flex items-center justify-center min-h-[200px] py-4 md:py-0 bg-neutral-white-100"
    >
      <div
        class="app-container flex flex-col md:flex-row items-center justify-between gap-6 md:gap-4 py-6 md:py-0"
      >
        <span class="flex flex-col gap-6">
          <h3 class="text-2xl font-bold text-neutral-900 text-start">
            {{ $t("index.newsletter.join_newsletter") }}
          </h3>
          <p class="text-neutral-500 text-sm font-normal">
            {{ $t("index.newsletter.newsletter_gift") }}
          </p>
        </span>
        <form action="" class="flex items-center justify-center gap-4">
          <input
            id="subscribe-email"
            type="email"
            name="subscribe-email"
            :placeholder="$t('index.newsletter.your_email')"
            class="bg-inherit border py-1.5 px-6 border-neutral-white-200 shadow-xs rounded-md focus:outline-none focus:bg-white text-neutral-300 placeholder:text-neutral-300"
          />
          <button
            type="submit"
            class="bg-neutral-900 rounded-md py-1.5 px-6 text-white"
          >
            {{ $t("index.newsletter.subscribe") }}
          </button>
        </form>
      </div>
    </div>
  </section>
</template>
<script setup>
import ProductCard from "~/components/products/ProductCard.vue";

const FEATURES_LIST = [
  {
    icon: "material-symbols-light:local-shipping-rounded",
    title: $t("index.features.free_shipping"),
    description: $t("index.features.free_shipping_desc"),
  },
  {
    icon: "ph:seal-check-fill",
    title: $t("index.features.satisfaction_guarantee"),
    description: $t("index.features.satisfaction_guarantee_desc"),
  },
  {
    icon: "mdi:secure",
    title: $t("index.features.secure_payment"),
    description: $t("index.features.secure_payment_desc"),
  },
];
</script>
