<template>
<header class="header">
    <div class="container"> 
        <div class="wraper">
        <nav class="nav">
            <img src="@/assets/images/logo-robot.png" class="logo">
            <div class="menu">
                <a href="#">О нас</a>
                <a href="#">Курсы</a>
                <a href="#">Кружок робототехники</a>
                <a href="#">Билет в будущее</a>
                <a href="#">Контакты</a>
                <a class="btn" href="#">Записаться на урок</a>
            </div>
        </nav>
</div>

    </div>
</header>
</template>

<style>


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
}

.logo {
    width: 65px;
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
