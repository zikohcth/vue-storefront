<template>
  <router-link :to="localizedRoute('/')" :title="$t('Home Page')" class="no-underline inline-flex">
    <img
      :width="width"
      :height="height"
      src="/assets/logo.svg"
      alt="Vuestore logo"
    >
  </router-link>
</template>

<script>
import Logo from 'core/components/Logo'

export default {
  mixins: [Logo],
  props: {
    width: {
      type: [String, Number],
      required: true
    },
    height: {
      type: [String, Number],
      required: true
    }
  }
}
</script>
