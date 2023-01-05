<template>
    <div>
        <span className="name">{{name}}</span>
        <span className="handle">@{{handle}}</span>
    </div>
</template>

<script setup>
    const props = defineProps(["name", "handle"]);
</script>

<style lang="scss" scoped>

</style>