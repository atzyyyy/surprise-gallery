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
          src: "/public/images/image1.jpg",
        },
        {
          id: 2,
          src: "/public/images/image2.jpg",
        },
        {
          id: 3,
          src: "/public/images/image3.jpg",
        },
        {
          id: 4,
          src: "/public/images/image4.jpg",
        },
        {
          id: 5,
          src: "/public/images/image5.jpg",
        },
        {
          id: 6,
          src: "/public/images/image6.jpg",
        },
        {
          id: 7,
          src: "/public/images/image7.jpg",
        },
        {
          id: 8,
          src: "/public/images/image8.jpg",
        },
        {
          id: 9,
          src: "/public/images/image9.jpg",
        },
        {
          id: 10,
          src: "/public/images/image10.jpg",
        },
        {
          id: 11,
          src: "/public/images/image11.jpg",
        },
        {
          id: 12,
          src: "/public/images/image12.jpg",
        },
        {
          id: 13,
          src: "/public/images/image13.jpg",
        },
        {
          id: 14,
          src: "/public/images/image14.jpg",
        },
        {
          id: 15,
          src: "/public/images/image15.jpg",
        },
        {
          id: 16,
          src: "/public/images/image16.jpg",
        },
        {
          id: 17,
          src: "/public/images/image17.jpg",
        },
        {
          id: 18,
          src: "/public/images/image18.jpg",
        },
        {
          id: 19,
          src: "/public/images/image19.jpg",
        },
        {
          id: 20,
          src: "/public/images/image20.jpg",
        },
        {
          id: 21,
          src: "/public/images/image21.jpg",
        },
        {
          id: 22,
          src: "/public/images/image22.jpg",
        },
        {
          id: 23,
          src: "/public/images/image23.jpg",
        },
        {
          id: 24,
          src: "/public/images/image24.jpg",
        },
        {
          id: 25,
          src: "/public/images/image25.jpg",
        },
        {
          id: 26,
          src: "/public/images/image26.jpg",
        },
        {
          id: 27,
          src: "/public/images/image27.jpg",
        },
        {
          id: 28,
          src: "/public/images/image28.jpg",
        },
        {
          id: 29,
          src: "/public/images/image29.jpg",
        },
        {
          id: 30,
          src: "/public/images/image30.jpg",
        },
        {
          id: 31,
          src: "/public/images/image31.jpg",
        },
        {
          id: 32,
          src: "/public/images/image32.jpg",
        },
        {
          id: 33,
          src: "/public/images/image33.jpg",
        },
        {
          id: 34,
          src: "/public/images/image34.jpg",
        },
        {
          id: 35,
          src: "/public/images/image35.jpg",
        },
        {
          id: 36,
          src: "/public/images/image36.jpg",
        },
        {
          id: 37,
          src: "/public/images/image37.jpg",
        },
        {
          id: 38,
          src: "/public/images/image38.jpg",
        },
        {
          id: 39,
          src: "/public/images/image39.jpg",
        },
        {
          id: 40,
          src: "/public/images/image40.jpg",
        },
        {
          id: 41,
          src: "/public/images/image41.jpg",
        },
        {
          id: 42,
          src: "/public/images/image42.jpg",
        },
        {
          id: 43,
          src: "/public/images/image43.jpg",
        },
        {
          id: 44,
          src: "/public/images/image44.jpg",
        },
        {
          id: 45,
          src: "/public/images/image45.jpg",
        },
        {
          id: 46,
          src: "/public/images/image46.jpg",
        },
        {
          id: 47,
          src: "/public/images/image47.jpg",
        },
        {
          id: 48,
          src: "/public/images/image48.jpg",
        },
        {
          id: 49,
          src: "/public/images/image49.jpg",
        },
        {
          id: 50,
          src: "/public/images/image50.jpg",
        },
        {
          id: 51,
          src: "/public/images/image51.jpg",
        },
        {
          id: 52,
          src: "/public/images/image52.jpg",
        },

      ]
      }
    },
  };
</script>