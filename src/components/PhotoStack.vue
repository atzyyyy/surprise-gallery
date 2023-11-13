<template>
  <swiper
  :effect="'cards'"
  :grabCursor="true"
  :modules="modules"
  :loop="true"
  >
    <swiper-slide
    v-for="(image, index) in images"
    :key="image.id"
    >
      <img :src="image.src" alt="">
    </swiper-slide>

  </swiper>
</template>

<script>
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  import 'swiper/css/effect-cards';

  import '../assets/_main.scss';

  // import required modules
  import { EffectCards } from 'swiper/modules';

  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [EffectCards],
      };
    },
    data() {
      return {
        images: [
        {
          id: 1,
          src: "/dist/images/image1.jpg",
        },
        {
          id: 2,
          src: "/dist/images/image2.jpg",
        },
        {
          id: 3,
          src: "/dist/images/image3.jpg",
        },
        {
          id: 4,
          src: "/dist/images/image4.jpg",
        },
        {
          id: 5,
          src: "/dist/images/image5.jpg",
        },
        {
          id: 6,
          src: "/dist/images/image6.jpg",
        },
        {
          id: 7,
          src: "/dist/images/image7.jpg",
        },
        {
          id: 8,
          src: "/dist/images/image8.jpg",
        },
        {
          id: 9,
          src: "/dist/images/image9.jpg",
        },
        {
          id: 10,
          src: "/dist/images/image10.jpg",
        },
        {
          id: 11,
          src: "/dist/images/image11.jpg",
        },
        {
          id: 12,
          src: "/dist/images/image12.jpg",
        },
        {
          id: 13,
          src: "/dist/images/image13.jpg",
        },
        {
          id: 14,
          src: "/dist/images/image14.jpg",
        },
        {
          id: 15,
          src: "/dist/images/image15.jpg",
        },
        {
          id: 16,
          src: "/dist/images/image16.jpg",
        },
        {
          id: 17,
          src: "/dist/images/image17.jpg",
        },
        {
          id: 18,
          src: "/dist/images/image18.jpg",
        },
        {
          id: 19,
          src: "/dist/images/image19.jpg",
        },
        {
          id: 20,
          src: "/dist/images/image20.jpg",
        },
        {
          id: 21,
          src: "/dist/images/image21.jpg",
        },
        {
          id: 22,
          src: "/dist/images/image22.jpg",
        },
        {
          id: 23,
          src: "/dist/images/image23.jpg",
        },
        {
          id: 24,
          src: "/dist/images/image24.jpg",
        },
        {
          id: 25,
          src: "/dist/images/image25.jpg",
        },
        {
          id: 26,
          src: "/dist/images/image26.jpg",
        },
        {
          id: 27,
          src: "/dist/images/image27.jpg",
        },
        {
          id: 28,
          src: "/dist/images/image28.jpg",
        },
        {
          id: 29,
          src: "/dist/images/image29.jpg",
        },
        {
          id: 30,
          src: "/dist/images/image30.jpg",
        },
        {
          id: 31,
          src: "/dist/images/image31.jpg",
        },
        {
          id: 32,
          src: "/dist/images/image32.jpg",
        },
        {
          id: 33,
          src: "/dist/images/image33.jpg",
        },
        {
          id: 34,
          src: "/dist/images/image34.jpg",
        },
        {
          id: 35,
          src: "/dist/images/image35.jpg",
        },
        {
          id: 36,
          src: "/dist/images/image36.jpg",
        },
        {
          id: 37,
          src: "/dist/images/image37.jpg",
        },
        {
          id: 38,
          src: "/dist/images/image38.jpg",
        },
        {
          id: 39,
          src: "/dist/images/image39.jpg",
        },
        {
          id: 40,
          src: "/dist/images/image40.jpg",
        },
        {
          id: 41,
          src: "/dist/images/image41.jpg",
        },
        {
          id: 42,
          src: "/dist/images/image42.jpg",
        },
        {
          id: 43,
          src: "/dist/images/image43.jpg",
        },
        {
          id: 44,
          src: "/dist/images/image44.jpg",
        },
        {
          id: 45,
          src: "/dist/images/image45.jpg",
        },
        {
          id: 46,
          src: "/dist/images/image46.jpg",
        },
        {
          id: 47,
          src: "/dist/images/image47.jpg",
        },
        {
          id: 48,
          src: "/dist/images/image48.jpg",
        },
        {
          id: 49,
          src: "/dist/images/image49.jpg",
        },
        {
          id: 50,
          src: "/dist/images/image50.jpg",
        },
        {
          id: 51,
          src: "/dist/images/image51.jpg",
        },
        {
          id: 52,
          src: "/dist/images/image52.jpg",
        },

      ]
      }
    },
  };
</script>