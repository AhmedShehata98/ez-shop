<template>
  <main class="w-full min-h-screen flex flex-col justify-start items-center">
    <div
      class="w-full flex items-center justify-center gap-3 bg-neutral-900 py-2.5 px-4"
    >
      <p class="text-white text-sm font-normal">
        Get 25% OFF on your first order.
      </p>
      <button type="button" class="text-white text-sm font-normal">
        Order Now
      </button>
    </div>
    <layout-app-header />
    <slot />
    <layout-app-footer />
  </main>
</template>
