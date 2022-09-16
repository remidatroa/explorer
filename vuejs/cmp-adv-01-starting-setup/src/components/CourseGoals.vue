<template>
  <ul>
    <li v-for="goal in goals" :key="goal">
        <slot :item="goal" another-prop="yoi"></slot>
    </li>
  </ul>
</template>

<script>
export default {
    data() {
        return {
            goals: ['Build app', 'learn new frameworks'],
        };
    },
};
</script>

<style>

</style>