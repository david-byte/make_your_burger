<template>
    <div class="message-container">
        {{msg}}
    </div>
</template>
<script>
export default {
   name: "Message",
   props: {
       msg: String
   }
}
</script>
<style scoped>

.message-container {
    color: #004085;
    background-color: #CCE5FF;
    border: 2px solid #B8DAFF;
    border-radius: 10px;
    padding: 15px;
    max-width: 400px;
    margin: 30px auto;
    text-align: center;
}
</style>