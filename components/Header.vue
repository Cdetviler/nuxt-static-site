<template>
  <div class="header-outer pt-4">
    <Wrapper>
      <header class="flex flex-row text-s">
        <div class="logo-area text-2xl">
          <nuxt-link to="/"> 
            Charlie Detviler
          </nuxt-link>
        </div>
        <nav class="ml-auto">
          <ul class="flex">
            <li class="header-link mr-6">
              <nuxt-link to="/"> Home </nuxt-link>
            </li>
            <li class="header-link mr-6">
              <nuxt-link class="text-base" to="/about"> About </nuxt-link>
            </li>
          </ul>
        </nav>
      </header>
    </Wrapper>
  </div>
</template>

<script>
  import Wrapper from '~/components/Wrapper.vue'

  export default {
    components: {
      Wrapper
    }
  }
</script>

<style>
  .header-outer {
    background-color: rgba(255,255,255,0.90);
    z-index: 1000;
    position: fixed;
    width: 100%;
  }

  .logo-area > a {
    color: theme('colors.grey.black');
  }

  .logo-area > a:hover {
    color: theme('colors.accent');
  }

  .header-link > a {
    display: block;
    position: relative;
    padding-bottom: 22px;
    padding-top: 1px;
    color: theme('colors.grey.light');
  }

  .header-link > a:after {
    content: '';
    position: absolute;
    left: 0;
    display: inline-block;
    height: 1.25em;
    width: 100%;
    border-top: 2px solid theme('colors.accent');
    bottom: -1px;
    opacity: 0;
    -webkit-transition: opacity 0.35s, -webkit-transform 0.35s;
    transition: opacity 0.35s, transform 0.35s;
    -webkit-transform: scale(0,1);
    transform: scale(0,1);
  }

  .header-link > a:hover:after,
  .header-link > .nuxt-link-exact-active:after {
    opacity: 1;
    -webkit-transform: scale(1);
    transform: scale(1);
  }

  .header-link > .nuxt-link-exact-active {
    color: theme('colors.accent');
  }
</style>
