<template>
  <section class="future-ticket">
    <div class="container">
      <div class="content-ticket">
        <div class="text-ticket">
          <h1>Билет в будущее!</h1>
          <h3>WorldSkills Russia</h3>
          <div class="line-ticket"></div>
          <p>
            Наша школа программирования и робототехники активно принимает участие
            в уникальном проекте WorldSkills "Билет в будущее". Это проект ранней
            профессиональной ориентации школьников 6–11 классов."Билет в будущее" 
            помогает детям найти свою индивидуальную траекторию, чтобы с раннего возраста начать развиваться 
            в своем направления и достигать вершин!
            <br /><br />
            Более подробную информацию смотрите на сайте:
            <br />
            <a href="http://bilet-help.worldskills.ru/" target="_blank">
              http://bilet-help.worldskills.ru/
            </a>
          </p>
        </div>

        <div class="image-ticket">
          <img src="@/assets/images/future-ticket.jpg" class="ticket-img">
        </div>

      </div>
    </div>
  </section>
</template>

<style>

.content-ticket {
  display: flex;
  justify-content: space-between;
  gap: 40px;
}

.future-ticket {
  padding: 80px;
}

.text-ticket {
  max-width: 800px;
  display: flex;
  flex-direction: column;
  text-align: center;
}

.text-ticket h1 {
  font-size: 50px;
  font-weight: 700;
  color: #3F1B62;
}

.text-ticket h3 {
  font-size: 18px;
  color: #7c7c7c;
  margin-top: 2px;
}

.line-ticket {
  width: 60px;
  height: 3px;
  background: #3F1B62;
  margin: 20px auto;
  border-radius: 3px;
}

.text-ticket p {
  font-size: 23px;
  line-height: 1.5;
  color: #000000;
}

.text-ticket a {
  color: #c26aff;
  font-size: 23px;
  text-decoration: none;
}
.image-ticket{
  padding: 80px;
}

.ticket-img {
  max-width: 500px;
  border-radius: 50px;
}

</style>