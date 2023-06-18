<script setup>
    import CategorySelect from '../components/CategorySelect.vue';
</script>

<template>
    <div class="p-8">
        <button
            type="button"
            class="text-white text-2xl font-semibold hover:underline cursor-pointer"
        >
            Browse all
        </button>

        <div class="py-1.5"></div>

        <div class="grid xl:grid-cols-5 lg:grid-cols-4 md:grid-cols-3 sm:grid-cols-2 gap-6">
            <CategorySelect category="Podcasts" image="https://picsum.photos/id/40/300/300"/>
            <CategorySelect category="Audiobooks" image="https://picsum.photos/id/45/300/300"/>
            <CategorySelect category="Made For You" image="https://picsum.photos/id/76/300/300"/>
            <CategorySelect category="New Release" image="https://picsum.photos/id/56/300/300"/>
            <CategorySelect category="Hot 10" image="https://picsum.photos/id/25/300/300"/>
            <CategorySelect category="Rock Music" image="https://picsum.photos/id/103/300/300"/>
            <CategorySelect category="Top 100" image="https://picsum.photos/id/244/300/300"/>
            <CategorySelect category="Pop Music" image="https://picsum.photos/id/202/300/300"/>
            <CategorySelect category="Popular Music" image="https://picsum.photos/id/101/300/300"/>
            <CategorySelect category="Hiphop Muic" image="https://picsum.photos/id/120/300/300"/>
            <CategorySelect category="Jazz and Blues" image="https://picsum.photos/id/40/300/300"/>
            <CategorySelect category="Rhythm Music" image="https://picsum.photos/id/45/300/300"/>
            <CategorySelect category="Classical Music" image="https://picsum.photos/id/76/300/300"/>
            <CategorySelect category="Country Muic" image="https://picsum.photos/id/56/300/300"/>
            <CategorySelect category="World Music" image="https://picsum.photos/id/25/300/300"/>
            <CategorySelect category="Heavy Metal" image="https://picsum.photos/id/103/300/300"/>
            <CategorySelect category="Folk Music" image="https://picsum.photos/id/244/300/300"/>
            <CategorySelect category="Funk Music" image="https://picsum.photos/id/202/300/300"/>
            <CategorySelect category="Disco" image="https://picsum.photos/id/101/300/300"/>
            <CategorySelect category="Latin" image="https://picsum.photos/id/120/300/300"/>
            <CategorySelect category="Podcasts" image="https://picsum.photos/id/40/300/300"/>
            <CategorySelect category="Salsa Music" image="https://picsum.photos/id/45/300/300"/>
            <CategorySelect category="Opera Music" image="https://picsum.photos/id/76/300/300"/>
            <CategorySelect category="Music of Africa" image="https://picsum.photos/id/56/300/300"/>
            <CategorySelect category="Music of India" image="https://picsum.photos/id/25/300/300"/>
            <CategorySelect category="New Wave" image="https://picsum.photos/id/103/300/300"/>
            <CategorySelect category="Acoustic Music" image="https://picsum.photos/id/244/300/300"/>
            <CategorySelect category="Made For You" image="https://picsum.photos/id/202/300/300"/>
            <CategorySelect category="College Rock" image="https://picsum.photos/id/101/300/300"/>
            <CategorySelect category="Soul Music" image="https://picsum.photos/id/120/300/300"/>
            <CategorySelect category="Classical Blues" image="https://picsum.photos/id/40/300/300"/>
            <CategorySelect category="Hindi Songs" image="https://picsum.photos/id/45/300/300"/>
            <CategorySelect category="Kannada Songs" image="https://picsum.photos/id/76/300/300"/>
            <CategorySelect category="Electronic Dance" image="https://picsum.photos/id/56/300/300"/>
            <CategorySelect category="Polka Music" image="https://picsum.photos/id/25/300/300"/>
            <CategorySelect category="Signature Songs" image="https://picsum.photos/id/103/300/300"/>
            <CategorySelect category="To Remember" image="https://picsum.photos/id/244/300/300"/>
            <CategorySelect category="Forever Classic" image="https://picsum.photos/id/202/300/300"/>
            <CategorySelect category="Punk Rock" image="https://picsum.photos/id/101/300/300"/>
            <CategorySelect category="Indie Rock" image="https://picsum.photos/id/120/300/300"/>
        </div>
    </div>
</template>
