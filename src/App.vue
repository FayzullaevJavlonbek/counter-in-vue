<template>
    <div class="container">
        <h1>Counter: {{ counter }}</h1>
        <button v-on:click="Add" class="btn btn-success">Add</button>
        <button @click="Delete" class="btn btn-danger">Delete</button>
    </div>
</template>

<script>
export default {
    data(){
        return {
            counter: 0,
        }
    },
    methods: {
        Add(){
            this.counter +=1
        },
        Delete(){
            this.counter -=1
        }
    }
}
</script>

<style></style>