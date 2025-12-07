<template>
    <section class="banner">
        <div class="banner-wave2">
            <img src="@/assets/images/wave.svg" alt="">
        </div>
        <div class="container">
            <div class="banner-content">
                <div>
                    <h1>Школа Программирования <br>
            и Роботехники</h1>
            <form class="banner-form">
            <input type="tel" placeholder="+7 999-999-99-99">
            <input type="text" placeholder="Имя">
            <button>Заказать звонок</button>
            </form>
                </div>
                <div class="banner-image">
                    <img src="@/assets/images/robot.gif" alt="">
                </div>
            </div>
        </div>
        <div class="banner-wave1">
            <img src="@/assets/images/wave.svg" alt="">
        </div>
    </section>
</template>

<style>
.container {
    max-width: 1290px;
    margin: 0 auto;
}
.banner {
    position: relative;
}
.banner-content {
    display: flex;
    justify-content: space-between;
}

.banner-content h1 {
    font-size: 40px;
    font-weight: 800;
    line-height: 1.2;
    color: #3F1B62;
    text-transform:uppercase;
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
    position: relative;
    left: calc(30% - 90px);
}
.banner-image {
    max-width: 560px;
}
</style>