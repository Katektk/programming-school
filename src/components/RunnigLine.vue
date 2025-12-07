<template>
  <div class="marquee">
  <div class="marquee-track">
    <div class="marquee-content">
      <span>• Присоединяйся •&nbsp;</span>
      <span>• Присоединяйся •&nbsp;</span>
      <span>• Присоединяйся •&nbsp;</span>
      <span>• Присоединяйся •&nbsp;</span>
    </div>
    <div class="marquee-content">
      <span> Присоединяйся •&nbsp;</span>
      <span>• Присоединяйся •&nbsp;</span>
      <span>• Присоединяйся •&nbsp;</span>
      <span>• Присоединяйся •&nbsp;</span>
    </div>
    <div class="marquee-content">
      <span> Присоединяйся •&nbsp;</span>
      <span>• Присоединяйся •&nbsp;</span>
      <span>• Присоединяйся •&nbsp;</span>
      <span>• Присоединяйся •&nbsp;</span>
    </div>
  </div>
  </div>
</template>

<style>
.marquee {
  width: 100%;     
  height: 100px;  
  background-color: #6f239c;
  display: flex;
  align-items: center;
  overflow: hidden; 
  position: relative;
}

.marquee-track {
  display: flex;
  animation: scroll-left 20s linear infinite;
  white-space: nowrap;
 
  min-width: 200%; 
}

.marquee-content {
  display: flex;
  flex-shrink: 0; 
  flex: 0 0 50%; 
}

 .marquee-content span {
  white-space: nowrap;
  font-size: 20px;
  color: white;
  margin-right: 10px;
}

@keyframes scroll-left {
  from { transform: translateX(0); }
  to   { transform: translateX(-50%); }
}
</style>