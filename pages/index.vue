<template>
    <UContainer class="mx-auto">
        <div class="py-12 flex justify-center">
            <img src="/logo-header_blanc.png" class="h-auto max-w-full" alt="Laboratoire Carbonneaux logo" />
        </div>
        <div class=" flex justify-center py-6 grid grid-cols-5 gap-10">
            <Flipcard txtfront="Supra structure<br>transvissée<br>(Montréal)" txtback="blablaback"
                @click="isOpenmod1 = !isOpenmod1"></Flipcard>
            <Flipcard txtfront="PAC<br>implanto-portée" txtback="blablaback"></Flipcard>
            <Flipcard txtfront="PAC<br>mucco-portée" txtback="blablaback"></Flipcard>
            <Flipcard txtfront="Châssis<br>métallique<br>(PAPIM)" txtback="blablaback"></Flipcard>
            <Flipcard txtfront="Prothèse<br>combinée" txtback="blablaback"></Flipcard>
            <Flipcard txtfront="Flux<br>numérique" txtback="blablaback"></Flipcard>
            <Flipcard txtfront="Laboratoire" txtback="blablaback"></Flipcard>
            <Flipcard txtfront="Documents" txtback="blablaback"></Flipcard>
            <Flipcard txtfront="Livraisons" txtback="blablaback"></Flipcard>
            <Flipcard txtfront="Contact" txtback="blablaback"></Flipcard>

        </div>

        <UModal v-model="isOpenmod1">
            <UCard :ui="{ ring: '', divide: 'divide-y divide-gray-100 dark:divide-gray-800' }">
                <template #header>
                    <div class="text-lg">Supra structure transvissée (Montréal)</div>
                    <div class="text-[#939393]">Supra structure transvissée (Montréal)</div>
                </template>

                <div class="py-6 grid grid-cols-3 gap-10">
                    <img src="\suprastructure\IMG20220727140114.jpg" class="h-auto max-w-full cursor-pointer"
                        alt="Laboratoire Carbonneaux logo" />
                    <img src="\suprastructure\IMG20220727140130.jpg" class="h-auto max-w-full cursor-pointer"
                        alt="Laboratoire Carbonneaux logo" />
                    <img src="\suprastructure\IMG20220727140203.jpg" class="h-auto max-w-full cursor-pointer"
                        alt="Laboratoire Carbonneaux logo" />
                    <img src="\suprastructure\IMG20220727140214.jpg" class="h-auto max-w-full cursor-pointer"
                        alt="Laboratoire Carbonneaux logo" />
                    <img src="\suprastructure\IMG20220727140245.jpg" class="h-auto max-w-full cursor-pointer"
                        alt="Laboratoire Carbonneaux logo" />
                    <img src="\suprastructure\IMG20220727140300.jpg" class="h-auto max-w-full cursor-pointer"
                        alt="Laboratoire Carbonneaux logo" />
                </div>

            </UCard>
        </UModal>

    </UContainer>
</template>
<script setup>
const isOpenmod1 = ref(false)
</script>