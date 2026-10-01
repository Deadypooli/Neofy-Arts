<template>
    <Header />
    <div class="banana-hero" :style="{backgroundImage: 'url(' + heroImg + ')' }">
        <div class="banana-text">
            <h1>
                Banana Drama
            </h1>
            <p>
                RTS game · Steam
            </p>
            <p>
                by artifact design
            </p>
            <h3>
                DLC Character modeling and animation
            </h3>
        </div>
    </div>
        <div 
        v-for="(animal) in imgArray"
        :key="animal"
        class="banana-images">
            <img :src="animal[0]">
            <img :src="animal[1]">
        </div>
        <div class="vid-container">
            <video class="banana-video" autoplay muted loop playsinline>
                <source :src="vid" type="video/mp4">
                Your browser does not support the video tag.
            </video>
        </div>
</template>

<script>
    import Header from '@/components/Header.vue';
    import bananaHero from '@/img/bananaDrama/Banana-hero.webp';
    import tigerVid from'@/img/bananaDrama/tiger-cleaning.mp4';
    import cockatooFront from '@/img/bananaDrama/cockatoo-front.webp';
    import cockatooSide from '@/img/bananaDrama/cockatoo-side.webp';
    import cowFront from '@/img/bananaDrama/cow-front.webp';
    import cowSide from '@/img/bananaDrama/cow-side.webp';
    import giraffeFront from '@/img/bananaDrama/giraffe-front.webp';
    import giraffeSide from '@/img/bananaDrama/giraffe-side.webp';
    import lionFront from '@/img/bananaDrama/lion-front.webp';
    import lionSide from '@/img/bananaDrama/lion-side.webp';
    import tigerFront from '@/img/bananaDrama/tiger-front.webp';
    import tigerSide from '@/img/bananaDrama/tiger-side.webp';

    export default {
        components: { Header },
        name: 'BananaDrama',
        data() {
            return {
                heroImg: bananaHero,
                vid: tigerVid,
                imgArray: [
                    [
                        cockatooFront,
                        cockatooSide
                    ],
                    [
                        cowFront,
                        cowSide
                    ],
                    [
                        giraffeFront,
                        giraffeSide
                    ],
                    [
                        lionFront,
                        lionSide
                    ],
                    [
                        tigerFront,
                        tigerSide
                    ],
                ]
            };
        },
    };
</script>