<template>
    <section class="coursers">
        <div class="container">
            <h1 class="coursers-title">Наши курсы</h1>
            <p class="coursers-subtitle">При выборе курсов ориентируйтесь на интересы, возраст и увлечения вашего ребенка!</p>
            <div class="coursers-wrapper">
                <div class="coursers-card">
                    <div class="course-top">
                        <span class="course-name">UNITY 3D</span>
                    </div>
                    <div class="course-desc">
                        <p>
                        Курс по разработке приложений и игр. Подходит детям от 11 лет. Ребенок научится использовать инструмент, с помощью которого профессиональные программисты в ведущих мировых студиях создают знаменитые игры</p>
                        <img class="course-img" src="@/assets/images/Unity3D.gif" alt="" >
                    </div>
                    <div class="course-price">2500 ₽</div>
                    <button class="course-btn">записаться</button>
                </div>
                <div class="coursers-card">
                    <div class="course-top">
                        <span class="course-name">3D МОДЕЛИРОВАНИЕ</span>
                    </div>
                    <div class="course-desc">
                        <p>
                        В нашем курсе ребенок познакомится с основными инструментами и сделает первые шаги в просторный мир моделирования. Во время обучения каждый ребенок создаст собственные модели </p>
                        <img class="course-img" src="@/assets/images/hello3D.gif" alt="" >
                    </div>
                    <div class="course-price">2000 ₽</div>
                    <button class="course-btn">записаться</button>
                </div>
                <div class="coursers-card">
                    <div class="course-top">
                        <span class="course-name">WEB - MASTERING</span>
                    </div>
                    <div class="course-desc">
                        <p>
                        Под руководством опытных педагогов-практиков ребенок научится создавать информативные сайты, отличающиеся оригинальным графическим оформлением </p>
                        <img class="course-img" src="@/assets/images/web-mastering.gif" alt="" >
                    </div>
                    <div class="course-price">2000 ₽</div>
                    <button class="course-btn">записаться</button>
                </div>
                <div class="coursers-card">
                    <div class="course-top">
                        <span class="course-name">ДИЗАЙН-МЫШЛЕНИЕ</span>
                    </div>
                    <div class="course-desc">
                        <p>
                        Креативность и способность создавать есть во всех людях. Дизайн-мышление — это возможность реализовать и улучшить эти способности</p>
                        <img class="course-img" src="@/assets/images/rabbit.gif" alt="" >
                    </div>
                    <div class="course-price">2000 ₽</div>
                    <button class="course-btn">записаться</button>
                </div>
                <div class="coursers-card">
                    <div class="course-top">
                        <span class="course-name">ИГРЫ В JAVASCRIPT</span>
                    </div>
                    <div class="course-desc">
                        <p>
                        Программисты на Java очень востребованы и с каждым годом необходимость в них только возрастает. Подарите вашему ребенку возможность овладеть навыками перспективной профессии</p>
                        <img class="course-img" src="@/assets/images/JS.gif" alt="" >
                    </div>
                    <div class="course-price">2000 ₽</div>
                    <button class="course-btn">записаться</button>
                </div>
                <div class="coursers-card">
                    <div class="course-top">
                        <span class="course-name">СОЗДАНИЕ ИГР В ROBLOX STUDIO</span>
                    </div>
                    <div class="course-desc">
                        <p>
                        Roblox - это популярнейшая многопользовательская онлайн-игра, ориентированная на детей возрастом от 6 до 18 лет, которая совсем недавно предоставила возможность разрабатывать игры на собственной платформе!</p>
                        <img class="course-img" src="@/assets/images/Roblox.gif" alt="" >
                    </div>
                    <div class="course-price">2000 ₽</div>
                    <button class="course-btn">записаться</button>
                </div>
                <div class="coursers-card">
                    <div class="course-top">
                        <span class="course-name">СОЗДАНИЕ ИГР В MINECRAFT</span>
                    </div>
                    <div class="course-desc">
                        <p>
                        Minecraft – это игра, которую любят дети и взрослые по всему миру. Дружелюбная среда Minecraft – отличное место, чтобы изучать программирование.  </p>
                        <img class="course-img" src="@/assets/images/minecraft.gif" alt="" >
                    </div>
                    <div class="course-price">2000 ₽</div>
                    <button class="course-btn">записаться</button>
                </div>
                <div class="coursers-card">
                    <div class="course-top">
                        <span class="course-name">СОЗДАНИЕ ИГР В SCRATCH</span>
                    </div>
                    <div class="course-desc">
                        <p class="course-desc">
                        Ваш ребенок превратится из пользователя компьютерных игр и мультиков в их создателя! Мы рекомендуем курс каждому от 7 до 14 лет</p>
                        <img class="course-img" src="@/assets/images/scratch.gif" alt="" >
                    </div>
                    <div class="course-price">2000 ₽</div>
                    <button class="course-btn">записаться</button>
                </div>
            </div>
        </div>
            
    </section>
</template>

<style>

.coursers {
    text-align: center;
}
.coursers-title {
    font-size: 50px;
    font-weight: 800;
    margin-bottom: 10px;
    color: #3F1B62;
}
.coursers-subtitle {
    font-size: 25px;
    color: #3F1B62;
    max-width: 750px;
    margin: 0 auto 40px;
    font-weight: 700;
}
.coursers-wrapper {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    
    justify-content: center;
    gap: 60px;
    margin-top: 40px;
}
.course-card {
    width: 440px;
    text-align: left;
}
.course-top {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.course-name {
    padding: 10px 0;
    border: 3px solid #3F1B62;
    border-radius: 12px;
    font-size: 18px;
    font-weight: 700;
    width: 350px;
    color: #3F1B62;
    background-color: #f5e3ff;
}
.course-img {
    max-width: 300px;
    height: 170px;
    object-fit: contain;
}
.course-desc {
    margin-top: 20px;
    margin-bottom: 15px 0;
    font-size: 16px;
    line-height: 1.45;
    color: #000;
    display: flex;
    text-align: left;
}
.course-desc p {
    font-weight: 500;
}

.course-price {
    font-size: 18px;
    font-weight: 700;
    margin-bottom: 15px;
    color: #000;
    text-align: start;
}
.course-btn {
    display: block;
    background: #6F239C;
    color: white;
    padding: 10px 25px;
    border: none;
    border-radius: 25px;
    font-size: 15px;
    cursor: pointer;
    

}

</style>
