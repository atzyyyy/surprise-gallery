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
      <img :src="image.src" alt="" rel="preload">
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
          src: "/images/image1.jpg",
        },
        {
          id: 2,
          src: "/images/image2.jpg",
        },
        {
          id: 3,
          src: "/images/image3.jpg",
        },
        {
          id: 4,
          src: "/images/image4.jpg",
        },
        {
          id: 5,
          src: "/images/image5.jpg",
        },
        {
          id: 6,
          src: "/images/image6.jpg",
        },
        {
          id: 7,
          src: "/images/image7.jpg",
        },
        {
          id: 8,
          src: "/images/image8.jpg",
        },
        {
          id: 9,
          src: "/images/image9.jpg",
        },
        {
          id: 10,
          src: "/images/image10.jpg",
        },
        {
          id: 11,
          src: "/images/image11.jpg",
        },
        {
          id: 12,
          src: "/images/image12.jpg",
        },
        {
          id: 13,
          src: "/images/image13.jpg",
        },
        {
          id: 14,
          src: "/images/image14.jpg",
        },
        {
          id: 15,
          src: "/images/image15.jpg",
        },
        {
          id: 16,
          src: "/images/image16.jpg",
        },
        {
          id: 17,
          src: "/images/image17.jpg",
        },
        {
          id: 18,
          src: "/images/image18.jpg",
        },
        {
          id: 19,
          src: "/images/image19.jpg",
        },
        {
          id: 20,
          src: "/images/image20.jpg",
        },
        {
          id: 21,
          src: "/images/image21.jpg",
        },
        {
          id: 22,
          src: "/images/image22.jpg",
        },
        {
          id: 23,
          src: "/images/image23.jpg",
        },
        {
          id: 24,
          src: "/images/image24.jpg",
        },
        {
          id: 25,
          src: "/images/image25.jpg",
        },
        {
          id: 26,
          src: "/images/image26.jpg",
        },
        {
          id: 27,
          src: "/images/image27.jpg",
        },
        {
          id: 28,
          src: "/images/image28.jpg",
        },
        {
          id: 29,
          src: "/images/image29.jpg",
        },
        {
          id: 30,
          src: "/images/image30.jpg",
        },
        {
          id: 31,
          src: "/images/image31.jpg",
        },
        {
          id: 32,
          src: "/images/image32.jpg",
        },
        {
          id: 33,
          src: "/images/image33.jpg",
        },
        {
          id: 34,
          src: "/images/image34.jpg",
        },
        {
          id: 35,
          src: "/images/image35.jpg",
        },
        {
          id: 36,
          src: "/images/image36.jpg",
        },
        {
          id: 37,
          src: "/images/image37.jpg",
        },
        {
          id: 38,
          src: "/images/image38.jpg",
        },
        {
          id: 39,
          src: "/images/image39.jpg",
        },
        {
          id: 40,
          src: "/images/image40.jpg",
        },
        {
          id: 41,
          src: "/images/image41.jpg",
        },
        {
          id: 42,
          src: "/images/image42.jpg",
        },
        {
          id: 43,
          src: "/images/image43.jpg",
        },
        {
          id: 44,
          src: "/images/image44.jpg",
        },
        {
          id: 45,
          src: "/images/image45.jpg",
        },
        {
          id: 46,
          src: "/images/image46.jpg",
        },
        {
          id: 47,
          src: "/images/image47.jpg",
        },
        {
          id: 48,
          src: "/images/image48.jpg",
        },
        {
          id: 49,
          src: "/images/image49.jpg",
        },
        {
          id: 50,
          src: "/images/image50.jpg",
        },
        {
          id: 51,
          src: "/images/image51.jpg",
        },
        {
          id: 52,
          src: "/images/image52.jpg",
        },

      ]
      }
    },
  };
</script>