<template>
    <div >
        <img :src="원룸.image" class="room-img">
        <h4>{{원룸.title}}</h4>
        <p>{{원룸.price}} 원</p>
    </div> 
</template>

<script>
export default {
    name : 'CardKing',
    props : {
        원룸 : Object,
    }
}
</script>

<style>

</style>
