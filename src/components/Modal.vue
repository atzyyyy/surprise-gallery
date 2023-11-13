<script>
  export default {
    name: 'Modal',
    methods: {
      close() {
        this.$emit('close');
      },
    },
  };
</script>

<template>
  <transition name="modal-fade">
    <div class="modal-backdrop">
      <div class="modal"
        role="dialog"
        aria-labelledby="modalTitle"
        aria-describedby="modalDescription"
      >
          <button
            type="button"
            class="btn-close"
            @click="close"
            aria-label="Close modal"
          >
            x
          </button>

        <section
          class="modal-body"
          id="modalDescription"
        >
          <slot name="body"></slot>
        </section>

      </div>
    </div>
  </transition>
</template>

<style lang="scss">

  @import '../assets/_base.scss';

  .modal-backdrop {
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background-color: rgba(0, 0, 0, 0.3);
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .modal {
    width: 100vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .modal-body {
    padding: 20px;
    margin: auto;
    width: 90vw;
    height: auto;

    @media (min-width: 768px) {
      width: 35vw;
    }
  }

  .btn-close {
    position: absolute;
    top: 10px;
    right: 10px;
    border: none;
    font-size: 20px;
    padding: 10px;
    cursor: pointer;
    font-weight: bold;
    color: $accent-color-2;
    background: transparent;
  }

  .modal-fade-enter,
  .modal-fade-leave-to {
    opacity: 0;
  }

  .modal-fade-enter-active,
  .modal-fade-leave-active {
    transition: opacity .5s ease;
  }
</style>