<template>
  <div class="marquee-wrapper">
    <div class="marquee">
      • Присоединяйся • Присоединяйся • Присоединяйся • Присоединяйся • Присоединяйся • Присоединяйся • Присоединяйся • Присоединяйся • Присоединяйся •
    </div>
  </div>
</template>

<script>
export default {
  name: 'MarqueeText'
}
</script>

<style scoped>
.marquee-wrapper {
  width: 100%;
  overflow: hidden;
  background-color: #7B4BFF; /* фиолетовый фон */
}

.marquee {
  display: inline-block;
  white-space: nowrap;
  padding: 10px 0;
  color: white;
  font-weight: bold;
  animation: marquee 10s linear infinite;
}

@keyframes marquee {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(-100%);
  }
}
</style>