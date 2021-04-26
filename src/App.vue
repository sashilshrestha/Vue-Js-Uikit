<template>
    <Cards />
</template>

<script>
import Cards from './components/Cards';

export default {
    name: 'App',
    components: {
        Cards,
    },
};
</script>

<style lang="scss">
// 1. Your custom variables and variable overwrites.
$global-link-color: #da7d02;

// 2. Import default variables and available mixins.
@import '~uikit/src/scss/variables-theme.scss';
@import '~uikit/src/scss/mixins-theme.scss';

// 3. Your custom mixin overwrites.
@mixin hook-card() {
    color: #000;
}

// 4. Import UIkit.
@import '~uikit/src/scss/uikit-theme.scss';

// Some font smoothing
html {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-rendering: optimizeLegibility;
}

#app {
    font-family: Poppins;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
