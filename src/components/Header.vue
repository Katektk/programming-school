<template>
<header class="header">
    <div class="container2"> 
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

.container2 {
    max-width: 1300px;
    margin: 0 auto;
}


.wraper {
    margin: 0 auto;
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
    
}
.nav{
    flex-grow: 1;
    display: flex;
    gap: 107px;
}

.header {
    background-color: #3F1B62;
    position: absolute;
    top: 0;
    left: 50%;
    width: 100vw;
    transform: translateX(-50%);
    z-index: 0;
    overflow: visible;
}


.logo {
    width: 50px;
    height: auto;
}

.menu {
    display: flex;
    gap: 68px;
}

.menu a {
    color: white;
    text-decoration: none;
    font-size: 18px;
    font-weight: 600;
}

.btn {
    background-color: #ff007f;
    padding: 14px 32px;
    border-radius: 30px;
    color: white;
    font-weight: 700;
    text-decoration: none;
    font-size: 18px;
}

@media (max-width: 768px) {
    .nav {
        flex-direction: column;
        gap: 15px;
        padding: 10px;
    }

    .menu {
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
    }
}
</style>
