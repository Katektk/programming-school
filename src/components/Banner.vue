<template>
    <section class="banner">
        <div class="banner-content">
            <h1>Школа Программирования <br>
            и Роботехники</h1>
            <form class="banner-form">
            <input type="tel" placeholder="+7 999-999-99-99">
            <input type="text" placeholder="Имя">
            <button>Заказать звонок</button>
            </form>
        </div>
        <div class="fullwidth">
            <img class="banner-wave1" src="@/assets/images/wave.svg" alt="">
            <img class="banner-wave2" src="@/assets/images/wave.svg" alt="">
        </div>
        <div class="banner-image">
            <img src="@/assets/images/robot.gif" alt="">
        <img class=" elipse purple-elipse1"src="@/assets/images/purple_elipse.png" alt="" >
        <img class=" elipse purple-elipse2"src="@/assets/images/purple_elipse.png" alt="" >
        <img class="elipse pink-elipse1"src="@/assets/images/pink_elipse.png" alt="" >
        <img class="elipse pink-elipse2"src="@/assets/images/pink_elipse.png" alt="" >
        <img class="elipse pink-elipse3"src="@/assets/images/pink_elipse.png" alt="" >

        </div>


    </section>
    
</template>

<style>
.banner {
    position: relative;
    padding: 80px 0 150px;
    overflow: visible;
    display: flex;
    justify-content: space-between;
}

.banner-content h1 {
    font-size: 40px;
    font-weight: 800;
    line-height: 1.2;
    color: #3F1B62;
    text-transform:uppercase;
    margin-bottom: 50px;
}
.banner-form {
    display: flex;
    flex-direction: column;
    gap: 15px;
}
.banner-form input {
    width:350px;
    padding: 15px 20px;
    border-radius: 30px;
    border: none;
    font-size: 16px;
    outline: none;
    background: #f3e9ff;
}
.banner-form button {
    width: 200px;
    padding: 14px 0;
    border-radius: 30px;
    border: none;
    background: #6f239c;
    color: #fff;
    font-size: 16px;
    cursor: pointer;
    text-transform:uppercase;
    font-weight: 600;
    margin-left: 50px;
}
.banner-image {
    max-width: 560px;
}

.purple-elipse1 {
    position: absolute;
    left: -197px;
    top: -93px;
    width: 300px;
    height: 300px;
    margin-top: 20px;
}
.purple-elipse2 {
    position: absolute;
    width: 110px;
    height: 110px;
    top: 7px;
    right: -132px;
}
.pink-elipse1 {
    position: absolute;
    width: 200px;
    height: 200px;
    right: 321px;
    top: -32px;
}
.pink-elipse2 {
    position: absolute;
    width: 200px;
    height: 200px;
    bottom: -40px;
}
.pink-elipse3 {
    position: absolute;
    width: 200px;
    height: 200px;
    left: 1179px;
    top: 518px;
}
.fullwidth{
    position: absolute;
    top: 0;
    left: 50%;
    width: 100vw;
    height: 100%;
    transform: translateX(-50%);
    z-index: 0;
    overflow: visible;
}
.banner-wave1{
    width: 100%;
}
.banner-wave1{
    position: absolute;
    width: 100%;
    bottom: 70px
}







</style>