<template>
    <div class="card my-2 item-todo">
        <p>{{ item }}</p>
        <div v-on:click="removeItem" class="btn btn-danger btn-supr">X</div>
    </div>
</template>

<script>
export default {
    name: 'Item',
    props: ['item', 'removeItem']
}
</script>

<style scoped>
    .item-todo {
        position: relative;
        padding: 20px 60px 20px 30px;
        font-size: 20px;
        height: 90px;
    }
    .btn-supr{
        position: absolute;
        top: 10px;
        right: 10px
    }


</style>