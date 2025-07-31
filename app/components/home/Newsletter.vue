<template>
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
</template>
