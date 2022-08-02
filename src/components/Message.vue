<script>

export default ({
    name: 'Message',
    components: {},
    props: {
        initMessage: {
            type: String
        }
    },
    data() {
        return {
            message: ""
        }
    },
    mounted() {
        
        if(!this.message) {
            this.message = this.initMessage;
        }
    }
})
</script>

<template>
    <div class="card">
        <div class="card-content">{{ this.message }}</div>
    </div>
    <textarea 
        name="" 
        id="" 
        cols="100" 
        rows="10"
        >
    </textarea>
</template>

<style>
  .card {
    width: 32rem;
    border-radius: 0.5rem;
    background-color: #F8F8F8;
    box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
    padding: 1rem;
    margin-bottom: 2rem;
    border: 1px solid black;
  }
</style>