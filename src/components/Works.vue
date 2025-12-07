<template>
    <section class="education">
        <div class="container">
            <div class="education-wrapper">
                <h1 class="education-title" >Как проходит обучение</h1>
                <div class="eductaion-menu">
                    <div class="item-education">
                        <img class="img-education" src="@/assets/images/games.svg" alt="">
                        <p class="item-subtitle">Разрабатывают игры, пишут сайты и приложения, создают мультфильмы</p>
                    </div>
                    <div class="item-education">
                        <img class="img-education" src="@/assets/images/blogs.svg" alt="">
                        <p class="item-subtitle">Осваивают ораторское мастерство и ведут собственные видеоблоги</p>
                    </div>
                    <div class="item-education">
                        <img class="img-education" src="@/assets/images/idea.svg" alt="">
                        <p class="item-subtitle">Придумывают идеи для бизнеса и развивают предпринимательские навыки</p>
                    </div>
                    <div class="item-education">
                        <img class="img-education" src="@/assets/images/up.svg" alt="">
                        <p class="item-subtitle">Повышают компьютерную грамотность и узнают о безопасности в сети</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style>
.education {
    text-align: center;
}
.education-title {
    font-size: 50px;
    font-weight: 800;
    color: #3F1B62;
    margin-top: 30px;
}
.eductaion-menu {
    display: flex;
    gap: 35px;
}
.item-education {
    background-color:#e9d4ff;
    border-radius: 50px;
    max-width: 300px;
}
.item-subtitle {
    font-size: 25px;
    color: #19052e;
}
.img-education {
    max-width: 150px;
    margin-top: 30px;
}


</style>