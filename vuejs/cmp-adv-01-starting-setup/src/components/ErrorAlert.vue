<template>
    <dialog open>
        <slot></slot>
    </dialog>
</template>
<style  scoped>
    dialog{
        margin: 0px;
        position: fixed;
        top: 20vh;
        left: 30%;
        width: 40%;
        background-color: brown;
        color: aliceblue;
        padding: 15px;
    }

</style>