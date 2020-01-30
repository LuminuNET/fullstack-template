<template>
  <div id="app">
    <lm-header />
    <lm-custom-header />
    <router-view />
    <lm-custom-footer />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import { LmHeader } from '@luminu/components';
import LmCustomHeader from '@/components/layout/CustomStickyHeader.vue';
import LmCustomFooter from '@/components/layout/CustomFooter.vue';

export default Vue.extend({
  components: {
    LmCustomHeader,
    LmCustomFooter,
    LmHeader,
  },
});
</script>

<style lang="scss">
@import '~@luminu/core/scss/_globals.scss';
</style>
