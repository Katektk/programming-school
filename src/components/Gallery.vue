<template>
  <div class="carousel">
    <div class="carousel-wrapper">
      <button class="arrow-left" @click="prev">&#10094;</button>
      
      <div class="carousel-images">
        <img :src="images[prevImage]" class="side left" />
        <img :src="images[currentImage]" class="main" />
        <img :src="images[nextImage]" class="side right" />
      </div>
    
      <button class="arrow-right" @click="next">&#10095;</button>
    </div>

    <div class="dots">
      <span 
        v-for="(img, image) in images" 
        :key="image" 
        :class="{active: image === currentImage}" 
        @click="goTo(image)">
      </span>
    </div>
  </div>
</template>

<script>
  
import childs from '@/assets/images/childs.jpg'
import desk from '@/assets/images/desk.jpg'
import group from '@/assets/images/group.jpg'
import list from '@/assets/images/list.jpg'

export default {
  data() {
    return {
      images: [childs, desk, group, list],
      currentImage: 0,
      intervalId: null
    };
  },
  
  computed: {
    prevImage() {
      return (this.currentImage - 1 + this.images.length) % this.images.length;
    },
    nextImage() {
      return (this.currentImage + 1) % this.images.length;
    }
  },
  methods: {
    next() {
      this.currentImage = this.nextImage;
    },
    prev() {
      this.currentImage = this.prevImage;
    },
    goTo(index) {
      this.currentImage = index;
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