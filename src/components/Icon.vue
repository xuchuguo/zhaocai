<template>
    <svg class="icon">
        <use :xlink:href="'#' + name"></use>
    </svg>
</template>

<script>
import '@/assets/svg.js'
    export default {
        props:[
            'name'
        ]
    }
</script>

<style lang="scss" scoped>
  .icon {
       width: 1em; height: 1em;
       vertical-align: -0.15em;
       fill: currentColor;
       overflow: hidden;
    }
</style>