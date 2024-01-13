<template>
    <div class="container flex justify-center">
        <div class="flip-card">
            <div class="flip-card-inner">
                <div
                    class="flip-card-front rounded-lg box-border border border-[#f0f8c3] bg-[#A4BE26] flex justify-center items-center cursor-pointer text-center">
                    <h1 v-html="txtfront"></h1>
                </div>
                <div
                    class="flip-card-back rounded-lg box-border border border-[#f0f8c3] bg-[#637217] flex justify-center items-center cursor-pointer text-center">
                    <h1 v-html="txtback"></h1>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
const props = defineProps(['txtfront', 'txtback'])
const { txtfront, txtback } = toRefs(props)
</script>

<style scoped>
.flip-card {
    width: 130px;
    height: 130px;
}

.flip-card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.8s;
    transform-style: preserve-3d;
}

.container:hover .flip-card-inner {
    transform: rotateY(180deg);
}

.flip-card-front,
.flip-card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    backface-visibility: hidden;
}


.flip-card-back {
    transform: rotateY(180deg);
}
</style>