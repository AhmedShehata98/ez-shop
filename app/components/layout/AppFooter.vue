<template>
  <footer class="w-full py-8">
    <div
      class="app-container grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 md:gap-8 lg:gap-14 py-20"
    >
      <!-- logo and description -->
      <div class="flex flex-col items-start justify-start gap-3.5 mt-4">
        <h3 class="text-xl font-bold text-neutral-900 capitalize text-start">
          {{ $t("layout.AppFooter.title") }}
        </h3>
        <p class="font-normal text-sm capitalize text-neutral-500">
          {{ $t("layout.AppFooter.desc") }}
        </p>
      </div>
      <!-- website links -->
      <ul class="w-full grid grid-cols-2 md:grid-cols-3 gap-3 md:gap-6">
        <div class="flex flex-col gap-9">
          <h4 class="text-neutral-300 font-medium">
            {{ $t("layout.AppFooter.sections.shop") }}
          </h4>
          <ul class="grid grid-flow-row-dense gap-4 text-neutral-500">
            <nuxt-link href="#" class="text-inherit font-medium">
              {{ $t("layout.AppFooter.sections.my_account") }}
            </nuxt-link>
            <nuxt-link href="#" class="text-inherit font-medium">
              {{ $t("layout.AppFooter.sections.checkout") }}
            </nuxt-link>
            <nuxt-link href="#" class="text-inherit font-medium">
              {{ $t("layout.AppFooter.sections.cart") }}
            </nuxt-link>
          </ul>
        </div>
        <div class="flex flex-col gap-9">
          <h4 class="text-neutral-300 font-medium">
            {{ $t("layout.AppFooter.sections.company") }}
          </h4>
          <ul class="grid grid-flow-row-dense gap-4 text-neutral-500">
            <nuxt-link href="/about-us" class="text-inherit font-medium">
              {{ $t("layout.AppFooter.sections.about_us") }}
            </nuxt-link>
            <nuxt-link href="/contact" class="text-inherit font-medium">
              {{ $t("layout.AppFooter.sections.contact") }}
            </nuxt-link>
            <nuxt-link href="/careers" class="text-inherit font-medium">
              {{ $t("layout.AppFooter.sections.careers") }}
            </nuxt-link>
          </ul>
        </div>
        <div class="flex flex-col gap-9">
          <h4 class="text-neutral-300 font-medium">
            {{ $t("layout.AppFooter.sections.support") }}
          </h4>
          <ul class="grid grid-flow-row-dense gap-4 text-neutral-500">
            <nuxt-link href="/faq" class="text-inherit font-medium">
              {{ $t("layout.AppFooter.sections.faq") }}
            </nuxt-link>
            <nuxt-link href="/terms-of-use" class="text-inherit font-medium">
              {{ $t("layout.AppFooter.sections.terms_of_use") }}
            </nuxt-link>
            <nuxt-link href="/privacy-policy" class="text-inherit font-medium">
              {{ $t("layout.AppFooter.sections.privacy_policy") }}
            </nuxt-link>
          </ul>
        </div>
      </ul>
      <!-- payment accept -->
      <div class="flex flex-col gap-8">
        <h3 class="text-neutral-300">
          {{ $t("layout.AppFooter.sections.accepted_payments") }}
        </h3>
        <ul class="w-full grid grid-cols-3 items-center justify-start gap-x-2">
          <li>
            <svg
              width="31"
              height="32"
              viewBox="0 0 31 32"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g clip-path="url(#clip0_5428_34)">
                <path
                  d="M15.017 22.85C13.3637 24.2432 11.27 25.005 9.108 25C4.078 25 0 20.97 0 16C0 11.03 4.078 7.00002 9.108 7.00002C11.363 7.00002 13.426 7.81002 15.017 9.15002C16.67 7.75705 18.7633 6.99526 20.925 7.00002C25.955 7.00002 30.033 11.03 30.033 16C30.033 20.97 25.955 25 20.925 25C18.7633 25.0048 16.67 24.243 15.017 22.85Z"
                  fill="#ED0006"
                />
                <path
                  d="M15.017 22.85C16.0186 22.0115 16.8242 20.9636 17.377 19.7801C17.9299 18.5966 18.2166 17.3063 18.217 16C18.217 13.257 16.975 10.8 15.017 9.15002C16.67 7.75705 18.7633 6.99526 20.925 7.00002C25.955 7.00002 30.033 11.03 30.033 16C30.033 20.97 25.955 25 20.925 25C18.7633 25.0048 16.67 24.243 15.017 22.85Z"
                  fill="#F9A000"
                />
                <path
                  d="M15.017 22.85C16.975 21.2 18.217 18.743 18.217 16C18.217 13.257 16.975 10.8 15.017 9.15002C14.0154 9.98856 13.2098 11.0365 12.657 12.22C12.1041 13.4035 11.8174 14.6938 11.817 16C11.817 18.743 13.058 21.2 15.017 22.85Z"
                  fill="#FF5E00"
                />
              </g>
              <defs>
                <clipPath id="clip0_5428_34">
                  <rect width="30.033" height="32" fill="white" />
                </clipPath>
              </defs>
            </svg>
          </li>
          <li>
            <svg
              width="47"
              height="12"
              viewBox="0 0 47 12"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M5.22396 0L0.032959 11.826H6.24796L7.01796 9.941H8.77896L9.54996 11.827H16.39V10.387L17 11.827H20.54L21.149 10.357V11.827H35.376L37.106 9.99L38.726 11.827L46.033 11.842L40.825 5.946L46.033 0H38.839L37.155 1.803L35.586 0H20.109L18.779 3.053L17.42 0H11.219V1.39L10.529 0H5.22596H5.22396ZM6.42696 1.68H9.45696L12.9 9.699V1.679H16.219L18.879 7.429L21.329 1.679H24.633V10.166H22.623L22.607 3.516L19.677 10.166H17.88L14.935 3.516V10.166H10.801L10.018 8.263H5.78296L5.00096 10.164H2.78696L6.42696 1.679V1.68ZM34.64 1.68H26.47V10.16H34.513L37.106 7.35L39.605 10.16H42.217L38.42 5.945L42.217 1.679H39.718L37.138 4.458L34.64 1.679V1.68ZM7.89996 3.115L6.50596 6.505H9.29396L7.90096 3.115H7.89996ZM28.487 4.985V3.435H33.585L35.809 5.912L33.486 8.404H28.487V6.712H32.944V4.986H28.487V4.985Z"
                fill="#016FD0"
              />
            </svg>
          </li>
          <li>
            <svg
              width="43"
              height="14"
              viewBox="0 0 43 14"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M27.515 7.91772e-05C28.5598 -0.00452076 29.5959 0.191351 30.567 0.577079L30.104 3.50308L29.796 3.36008C29.003 2.9927 28.1355 2.81468 27.262 2.84008C25.919 2.84008 25.316 3.43108 25.302 4.00808C25.302 4.64308 26.032 5.06108 27.222 5.68108C29.182 6.64708 30.09 7.82908 30.077 9.37108C30.049 12.1841 27.725 14.0001 24.155 14.0001C22.629 13.9851 21.159 13.6531 20.361 13.2791L20.837 10.2361L21.285 10.4531C22.391 10.9581 23.119 11.1731 24.477 11.1731C25.457 11.1731 26.507 10.7551 26.52 9.84808C26.52 9.25608 26.073 8.82408 24.757 8.16008C23.469 7.51108 21.747 6.43008 21.775 4.48408C21.789 1.84508 24.155 7.91772e-05 27.515 7.91772e-05ZM14.831 13.7981H18.233L20.361 0.246079H16.959L14.831 13.7981Z"
                fill="#00579F"
              />
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M39.288 0.246079H36.657C35.845 0.246079 35.229 0.491079 34.878 1.37008L29.825 13.7981H33.395L34.109 11.7651H38.477C38.575 12.2411 38.883 13.7981 38.883 13.7981H42.033L39.288 0.246079ZM35.088 8.99608L36.448 5.20608C36.441 5.21608 36.486 5.09008 36.552 4.90108C36.65 4.62108 36.795 4.20808 36.895 3.90808L37.132 5.07508C37.132 5.07508 37.777 8.31908 37.917 8.99708H35.089L35.088 8.99608Z"
                fill="#00579F"
              />
              <path
                d="M8.65696 9.48708L11.989 0.246079H15.587L10.239 13.7841H6.64096L3.58896 1.93208C5.74496 3.10008 7.67696 5.45008 8.29296 7.61208L8.65696 9.48708Z"
                fill="#00579F"
              />
              <path
                d="M5.56296 0.246079H0.0889592L0.032959 0.519079C4.30296 1.64408 7.13096 4.35508 8.29296 7.61308L7.10296 1.38508C6.90696 0.519079 6.30496 0.275079 5.56296 0.245079V0.246079Z"
                fill="#FAA61A"
              />
            </svg>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>
