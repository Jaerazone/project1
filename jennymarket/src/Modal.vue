<template>
    <div class="black-bg" v-if= "모달창열렸니 == true" >
        <div class="white-bg">
            <img :src="원룸들[누른거].image" style="width:100%">
            <h4>{{ 원룸들[누른거].title }}</h4>
            <p>{{ 원룸들[누른거].content }} </p>
            <p>{{ 원룸들[누른거].price }} </p>
            <!-- <button @click= "모달창열렸니 = false">닫기</button> -->
        </div>
    </div>
</template>

<script>
export default {
    name : 'ModalChang',
    props : {
        원룸들 : Array,
        누른거 : Number,
        모달창열렸니 : Boolean
        // 첫글자 대문자로, Object 등등 문자면String 숫자면 Number 배열Array, true.false Boolean
        // (디버깅용으로쓴다. 자료형맞는지 확인하기위한 공간)
    }
}
</script>

<style>

</style>