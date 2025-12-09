<template>
    <footer class="footer">
        <div class="container">
            <div class="footer-wrapper">
                <div class="left-footer">
                    <h3 class="footer-title" >Контакты</h3>
                    <div class="contacts">
                    <a class="footer-phone" href="tel:+7 927 268-50-15">+7 927 268-50-15</a>
                    <a href="malito:vkonst@inbox.ru" class="footer-phone">vkonst@inbox.ru</a>
                    </div>
                    <div class="adress">
                        <h3 class="footer-title" >Адрес</h3>
                        <div class="footer-adress">
                            Белорусская улица, 6, Центральный район, Тольятти
                        </div>
                    </div>
                </div>
                <div class="right-wrapper">
                    <iframe src="https://yandex.ru/map-widget/v1/?um=constructor%3A0b34477627d35662a4c390d61e0ceaefa8761e2219fb7cb0b2bcd0599a3f7197&amp;source=constructor" width="591" height="302" frameborder="0"></iframe>
                </div>
            </div>
        </div>
    </footer>
</template>

<style>

.footer {
    background-color:#6f239c;
}
.footer-wrapper {
    display: flex;
    justify-content: space-between;
    padding: 20px 0;
    margin-top: 20px;
}
.footer-title {
    color: white;
    font-size: 28px;
}
.footer-phone {
    display: block;
    font-size: 20px;
    color: white;
    text-decoration: none;
    line-height: 190%;
}
.footer-phone:hover {
    color: #ff007f;
}
.footer-adress {
    color: white;
    font-size: 20px;
}


</style>