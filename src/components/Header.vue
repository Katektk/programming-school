<template>
<header class="header">
    <div class="container"> 
        <div class="wraper">
        <nav class="nav">
            <img src="@/assets/images/logo-robot.png" class="logo">
            <div class="menu">
          <a @click="scrollTo('our-courses')">Курсы</a>
          <a @click="scrollTo('robotics-club')">Кружок робототехники</a>
          <a @click="scrollTo('ticket')">Билет в будущее</a>
          <a @click="scrollTo('footer')">Контакты</a>
          <a class="btn" @click="scrollTo('signup')">Записаться на урок</a>
            </div>
        </nav>
</div>
</div>
</header>
</template>
<script>
export default {
  methods: {
    scrollTo(id) {
      const el = document.getElementById(id)
      if (!el) return

      const headerHeight = 100
      const y =
        el.getBoundingClientRect().top +
        window.pageYOffset -
        headerHeight

      window.scrollTo({
        top: y,
        behavior: 'smooth'
      })
    }
  }
}
</script>

<style>

.html {
  scroll-behavior: smooth;
}

.wraper {
    margin: 0 auto;
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav {
    display: flex;
    align-items: center;
    justify-content: space-between; 
    gap: 45px 
}

.header {
  background-color: #3F1B62;
  position: fixed;   /* ← ВОТ ЭТО ЗАКРЕПЛЕНИЕ */
  top: 0;            /* ← прижимаем к верху */
  left: 0;
  width: 100%;       /* ← на всю ширину */
  height: 80px;
  background-color: #3F1B62;
  z-index: 1000;     
}

.logo {
    width: 50px;
    height: auto;
}

.menu {
    display: flex;
    gap: 49px;
}

.menu a {
    color: white;
    text-decoration: none;
    font-size: 22px;
    font-weight: 600;
    flex-shrink: 0;
}

.btn {
    background-color: #ff007f;
    padding: 10px 50px;
    border-radius: 30px;
    color: white;
    font-weight: 700;
    text-decoration: none;
    font-size: 23px;
}
</style>
