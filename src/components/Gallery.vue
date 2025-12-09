<template>
  <div class="carousel">
    <div class="carousel-wrapper">
      <button class="arrow left" @click="prev">&#10094;</button>
      
      <div class="carousel-images">
        <img :src="images[prevIndex]" class="side left" />
        <img :src="images[currentIndex]" class="main" />
        <img :src="images[nextIndex]" class="side right" />
      </div>
    
      <button class="arrow right" @click="next">&#10095;</button>
    </div>

   
    <div class="dots">
      <span 
        v-for="(img, index) in images" 
        :key="index" 
        :class="{active: index === currentIndex}" 
        @click="goTo(index)">
      </span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
     images: [
     require('@/assets/images/childs.jpg'),
     require('@/assets/images/desk.jpg'),
     require('@/assets/images/group.jpg'),
     require('@/assets/images/list.jpg')]
    };
  },
  computed: {
    prevIndex() {
      return (this.currentIndex - 1 + this.images.length) % this.images.length;
    },
    nextIndex() {
      return (this.currentIndex + 1) % this.images.length;
    },
  },
  methods: {
    next() {
      this.currentIndex = this.nextIndex;
    },
    prev() {
      this.currentIndex = this.prevIndex;
    },
    goTo(index) {
      this.currentIndex = index;
    },
    startAutoSlide() {
      this.intervalId = setInterval(this.next, 1000);
    },
    stopAutoSlide() {
      clearInterval(this.intervalId);
    }
  },
  mounted() {
    this.startAutoSlide();
  },
  beforeUnmount() {
    this.stopAutoSlide();
  }
}
</script>

<style>
.carousel {
  width: 600px;
  margin: 0 auto;
  text-align: center;
  position: relative;
}

.carousel-wrapper {
  display: flex;
  align-items: center;
  position: relative;
}

.arrow {
  font-size: 30px;
  background: none;
  border: none;
  cursor: pointer;
  z-index: 10;
}

.carousel-images {
  display: flex;
  align-items: center;
  overflow: hidden;
}

.carousel-images img {
  transition: all 0.5s;
}

.carousel-images img.main {
  width: 300px;
  margin: 0 20px;
}

.carousel-images img.side {
  width: 100px;
  opacity: 0.5;
}

.carousel-images img.side.left {
  margin-right: 10px;
}

.carousel-images img.side.right {
  margin-left: 10px;
}

.dots {
  margin-top: 10px;
}

.dots span {
  display: inline-block;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: #ccc;
  margin: 0 5px;
  cursor: pointer;
}

.dots span.active {
  background: #333;
}
</style>