<template>
  <section class="w-full flex flex-col items-start justify-start">
    <div class="w-full flex items-center justify-start bg-neutral-white-100">
      <ul class="app-container flex items-center justify-start gap-2.5 py-4">
        <li class="text-sm font-medium capitalize text-neutral-500">
          <nuxt-link :href="localePath('/')">home</nuxt-link>
        </li>
        <Icon name="tabler:chevron-right" />
        <li class="text-sm font-medium capitalize text-neutral-900">search</li>
      </ul>
    </div>
    <div
      class="relative app-container flex items-start justify-start mt-8 gap-5"
    >
      <aside
        class="max-md:w-full md:w-64 h-fit shrink-0 flex flex-col items-start justify-start gap-y-10 px-4 py-6 border border-neutral-100 rounded-md"
      >
        <!-- category filter -->
        <div class="w-full">
          <h5
            class="text-sm font-medium text-neutral-900 text-start capitalize"
          >
            category
          </h5>
          <ul
            class="w-full grid grid-flow-row-dense gap-1 divide-y divide-neutral-white-200"
          >
            <li class="w-full flex items-center justify-start gap-2 py-3">
              <label
                for="sports"
                class="w-full flex items-center justify-start gap-2"
              >
                <input
                  id="sports"
                  type="checkbox"
                  name="sports"
                  class="accent-primary-800"
                />
                <p class="text-sm font-normal text-neutral-600 capitalize">
                  sports
                </p>
              </label>
            </li>
            <li class="w-full flex items-center justify-start gap-2 py-3">
              <label
                for="electronics"
                class="w-full flex items-center justify-start gap-2"
              >
                <input
                  id="electronics"
                  type="checkbox"
                  name="electronics"
                  class="accent-primary-800"
                />
                <p class="text-sm font-normal text-neutral-600 capitalize">
                  electronics
                </p>
              </label>
            </li>
            <li class="w-full flex items-center justify-start gap-2 py-3">
              <label
                for="mobiles-&-tablets"
                class="w-full flex items-center justify-start gap-2"
              >
                <input
                  id="mobiles-&-tablets"
                  type="checkbox"
                  name="mobiles-&-tablets"
                  class="accent-primary-800"
                />
                <p class="text-sm font-normal text-neutral-600 capitalize">
                  mobiles & tablets
                </p>
              </label>
            </li>
          </ul>
        </div>
        <div class="w-full flex flex-col items-start justify-start gap-3">
          <h5
            class="text-sm font-medium text-neutral-900 text-start capitalize"
          >
            colors
          </h5>
          <ul class="w-full grid grid-4 md:grid-cols-5 lg:grid-cols-6 gap-2.5">
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
        <div class="w-full flex flex-col items-start justify-start gap-3">
          <h5
            class="text-sm font-medium text-neutral-900 text-start capitalize"
          >
            sizes
          </h5>
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
        <div class="w-full flex flex-col items-start justify-start gap-3">
          <h5
            class="text-sm font-medium text-neutral-900 text-start capitalize"
          >
            price
          </h5>
          <input
            id="price"
            class="w-full accent-neutral-700"
            type="range"
            name="price"
            multiple
            step="0.1"
          />
        </div>
      </aside>
      <!-- search result wrapper -->
      <div class="w-[calc(100%-17rem)] flex flex-col items-start justify-start">
        <div class="w-full flex flex-col items-start justify-start gap-3">
          <h5 class="text-sm font-medium capitalize text-neutral-900">
            Applied Filters:
          </h5>
          <ul class="flex items-center justify-start gap-2.5 mb-7">
            <li
              class="flex items-center justify-center gap-1.5 border border-neutral-100 px-3 py-1 rounded-full"
            >
              <p class="text-xs font-medium uppercase text-neutral-900">
                Perfume
              </p>
              <button type="button">
                <Icon name="jam:close" />
              </button>
            </li>
            <li
              class="flex items-center justify-center gap-1.5 border border-neutral-100 px-3 py-1 rounded-full"
            >
              <p class="text-xs font-medium uppercase text-neutral-900">
                Size: M
              </p>
              <button type="button">
                <Icon name="jam:close" />
              </button>
            </li>
          </ul>
          <span class="w-full flex items-center justify-between gap-5">
            <p class="text-sm font-medium text-neutral-500 capitalize">
              Showing 1-9 of 36 results.
            </p>
            <select id="sort" name="sort">
              <option value="sort-by">sort by</option>
              <option value="asc">asc</option>
              <option value="desc">desc</option>
            </select>
          </span>
        </div>
        <div class="w-full flex flex-col mt-8">
          <ul
            class="w-full grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 md:gap-6"
          >
            <ProductsProductCard />
            <ProductsProductCard />
            <ProductsProductCard />
            <ProductsProductCard />
            <ProductsProductCard />
            <ProductsProductCard />
            <ProductsProductCard />
            <ProductsProductCard />
            <ProductsProductCard />
            <ProductsProductCard />
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
const localePath = useLocalePath();
useHeadSafe({
  title: "e-commerce | Products list",
});
</script>
