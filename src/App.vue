<template>
  <main class="content-grid">
    <div class="spinner" v-show="loading">
      <SpinnerHeart :loading="loading" />
    </div>
    <div class="card" v-show="!loading">
      <h1>Dear babu,</h1>
      <p>Happy Babu Day!</p>
      <p>{{ message }}</p>
      <p>This could be a simple gift to cherish our memories together. Click the icon below for a surprise!</p>
      <h4>Love,</h4>
      <h4><em>Fourthram</em></h4>
    </div>

    <div class="photos" v-show="!loading">
      <img src="/public/image-icon.svg" alt="icon" width="40" height="40" @click="showModal">
      <Modal v-show="isOpen" @close="closeModal"> 
        <template v-slot:body>
          <PhotoStack />
        </template>
      </Modal>
    </div>
  </main>
</template>

<script>
  import SpinnerHeart from './components/SpinnerHeart.vue'
  import PhotoStack from './components/PhotoStack.vue'
  import Modal from './components/Modal.vue'
  export default {
    components: {
      SpinnerHeart,
      PhotoStack,
      Modal,
    },
    data() {
      return {
        loading: true,
        isOpen: false,
        message: `
        It has been 21 months since I gathered the courage to talk to you, and I have never regretted that moment. 
        I am always grateful to have you in my life. 
        I love you so much, babu. 
        Let's make this relationship last forever. `,
      }
    },

    mounted() {
      setTimeout(() => {
        this.loading = false
      }, 4000)
    },

    methods: {
      showModal() {
        this.isOpen = true
      },
      closeModal() {
        this.isOpen = false
      }
    }

  }
</script>

