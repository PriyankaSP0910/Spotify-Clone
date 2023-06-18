<script setup>
    import HomeCard from '../components/HomeCard.vue';
</script>

<template>
    <div class="p-8">
        <button
            type="button"
            class="text-white text-2xl font-semibold hover:underline cursor-pointer"
        >
            Podcasts to make you smarter
        </button>

        <div class="py-1.5"></div>

        <div class="flex items-center">
            <HomeCard image="https://picsum.photos/id/30/300/300" title="Healthy Habits" subTitle="Kicktart your Morning routine with Martin Burg." />
            <HomeCard image="https://picsum.photos/id/45/300/300" title="Bengaluru" subTitle="Explore Banglore with Satish Kumar." />
            <HomeCard class="md:block hidden" image="https://picsum.photos/id/65/300/300" title="Happiness" subTitle="Find the secret to happiness with Linda Ray." />
            <HomeCard class="lg:block hidden" image="https://picsum.photos/id/67/300/300" title="Nature's Beauty" subTitle="Explore Nature's beauty with Shamili Dixit." />
            <HomeCard class="xl:block hidden" image="https://picsum.photos/id/100/300/300" title="Pollution" subTitle="Destruction of Mother Nature with Roy Kay. " />
        </div>
    </div>

    <div class="p-8">
        <button
            type="button"
            class="text-white text-2xl font-semibold hover:underline cursor-pointer"
        >
        Recommended radio
        </button>

        <div class="py-1.5"></div>

        <div class="flex items-center">
            <HomeCard image="https://picsum.photos/id/120/300/300" title="91.1 FM" subTitle="Radio City" />
            <HomeCard image="https://picsum.photos/id/110/300/300" title="91.9 FM" subTitle="Radio Indigo" />
            <HomeCard class="md:block hidden" image="https://picsum.photos/id/221/300/300" title="92.7 FM" subTitle="Big FM" />
            <HomeCard class="lg:block hidden" image="https://picsum.photos/id/232/300/300" title="93.5 FM" subTitle="Red FM" />
            <HomeCard class="xl:block hidden" image="https://picsum.photos/id/187/300/300" title="94.3 FM" subTitle="Radio One" />
        </div>
    </div>

    <div class="p-8">
        <button
            type="button"
            class="text-white text-2xl font-semibold hover:underline cursor-pointer"
        >
        Recommended songs
        </button>

        <div class="py-1.5"></div>

        <div class="flex items-center">
            <HomeCard image="https://picsum.photos/id/88/300/300" title="Solitude" subTitle="Billie Holiday" />
            <HomeCard image="https://picsum.photos/id/243/300/300" title="Manimal" subTitle="Heskil Fent" />
            <HomeCard class="md:block hidden" image="https://picsum.photos/id/123/300/300" title="Rings" subTitle="Ariana Grande" />
            <HomeCard class="lg:block hidden" image="https://picsum.photos/id/121/300/300" title="Money" subTitle="Lisa Manoban" />
            <HomeCard class="xl:block hidden" image="https://picsum.photos/id/99/300/300" title="Neruda" subTitle="Pablo Neskua" />
        </div>
    </div>
</template>
