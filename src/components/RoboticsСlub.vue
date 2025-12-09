<template>
    <section class="robotics-club">
       <div class="container"> 
       <div class="image">
       <img src="@/assets/images/robot.png" class="robot">
        <div class="text">
          <h1>Кружок робототехники</h1>
          <p>
            Также в нашей школе проходят занятия по РОБОТОТЕХНИКЕ! 
            Ребята учатся собирать и управлять конструктором. 
            Придумывать новые модели, находить способы решения 
            трудных задач и развивать логическое мышление
          </p>
          <button class="btn">Узнать больше</button>
        </div>
       </div>
      </div>
    </section>
</template>

<style>

.container {
  max-width: 100%;
}

.robotics-club {
  padding: 80px 0;
}

.image {
  display: flex;
  justify-content: space-between;
  gap: 30px;
}

.robot {
  max-width: 550px;
  height: 550px;
  object-fit: contain;
}

.text {
  max-width: 660px;
  text-align: center;
}

.text h1 {
  font-size: 50px;
  color: #3F1B62;
  margin-bottom: 20px;
  text-align: center;
}

.text p {
  font-size: 30px;
  line-height: 1.5;
  text-align: center;
}

.btn {
  background: #6f239c;
  color: white;
  border: none;
  border-radius: 40px;
  padding: 16px 40px;
  font-size: 16px;
  cursor: pointer;
  align-self: center;
  
}

.btn:hover {
  opacity: 0.85;
}
</style>