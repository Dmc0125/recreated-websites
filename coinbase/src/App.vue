<template>
  <main id="app" class="w-full min-h-screen bg-white pb-8">
    <div class="w-full min-h-20 p-2 bg-red-500 flex items-center justify-center">
      <svg
        style="color: currentColor"
        class="w-16 h-16 mr-2 flex-shrink-0"
        stroke-width=".9px"
        viewBox="0 0 24 24"
        fill="none"
      >
        <!-- eslint-disable max-len -->
        <path d="M12 19.5C16.1421 19.5 19.5 16.1421 19.5 12C19.5 7.85786 16.1421 4.5 12 4.5C7.85786 4.5 4.5 7.85786 4.5 12C4.5 16.1421 7.85786 19.5 12 19.5Z" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" />
        <path d="M11 15.5V12C11 11.7239 11.2239 11.5 11.5 11.5H12.5C12.7761 11.5 13 11.7239 13 12V15.5C13 15.7761 12.7761 16 12.5 16H11.5C11.2239 16 11 15.7761 11 15.5ZM12.9999 9C12.9999 9.55228 12.5522 10 11.9999 10C11.4476 10 10.9999 9.55228 10.9999 9C10.9999 8.44772 11.4476 8 11.9999 8C12.5522 8 12.9999 8.44772 12.9999 9Z" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" />
        <!-- eslint-enable max-len -->
      </svg>

      <p class="text-base font-medium">
        This is not real Coinbase website.
        For real Coinbase visit
        <a href="https://coinbase.com" rel="noopener" target="_blank">coinbase.com</a>
      </p>
    </div>

    <AppHeader />

    <router-view></router-view>

    <AppFooter />
  </main>
</template>

<script>
import AppHeader from '@/components/header/Header.vue';
import AppFooter from '@/components/footer/Footer.vue';

export default {
  components: {
    AppHeader,
    AppFooter,
  },
};
</script>

<style src="./assets/css/tailwind.css"></style>

<style>
@font-face {
  font-family: Roboto;
  font-weight: 300;
  src: url('/fonts/Roboto-Light.ttf');
}

@font-face {
  font-family: Roboto;
  font-weight: 400;
  src: url('/fonts/Roboto-Regular.ttf');
}

@font-face {
  font-family: Roboto;
  font-weight: 500;
  src: url('/fonts/Roboto-Medium.ttf');
}

@font-face {
  font-family: Roboto;
  font-weight: 700;
  src: url('/fonts/Roboto-Bold.ttf');
}

* {
  transition: all 200ms ease-in-out;
  font-family: Roboto, sans-serif;
}
</style>
