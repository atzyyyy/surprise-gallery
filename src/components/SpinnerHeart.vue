<template>
  <div v-show="loading" class="lds-heart" :style="{ width: `${size}px`, height: `${size}px` }">
      <div v-bind:style="[spinnerStyle]">
          <div class="div-before" v-bind:style="[spinnerStyle]"></div>
          <div class="div-after" v-bind:style="[spinnerStyle]"></div>
      </div>
  </div>
</template>

<script>

export default {
  name: 'HeartLoader',
  props: {
      loading: {
          type: Boolean,
          default: true,
      },
      size: {
          type: Number,
          default: 80,
      },
      color: {
          type: String,
          default: '#B0578D',
      },
      duration: {
          type: String,
          default: '1.2s',
      },
  },
  data() {
      return {
          spinnerStyle: {
              background: this.color,
              animationDuration: this.duration,
          },
      }
  },
}
</script>

<style scoped>
.lds-heart {
  display: inline-block;
  position: relative;
  margin: auto;

  transform: rotate(45deg);
  transform-origin: 50% 50%;
}
.lds-heart > div {
  top: 40%;
  left: 40%;
  position: absolute;
  width: 40%;
  height: 40%;
  background: #fff;
  animation-name: lds-heart;
  animation-timing-function: cubic-bezier(0.215, 0.61, 0.355, 1);
  animation-iteration-count: infinite;
}
.lds-heart .div-after,
.lds-heart .div-before {
  content: ' ';
  position: absolute;
  display: block;
  width: 100%;
  height: 100%;
  background: #fff;
}
.lds-heart .div-before {
  left: -75%;
  border-radius: 50% 0 0 50%;
}
.lds-heart .div-after {
  top: -75%;
  border-radius: 50% 50% 0 0;
}
@keyframes lds-heart {
  0% {
      transform: scale(0.95);
  }
  5% {
      transform: scale(1.1);
  }
  39% {
      transform: scale(0.85);
  }
  45% {
      transform: scale(1);
  }
  60% {
      transform: scale(0.95);
  }
  100% {
      transform: scale(0.9);
  }
}
</style>