<template>
    <section class="robotics-club">
       <div class="container"> 
       <div class="image-robotics">
       <img src="@/assets/images/robot.png" class="robot">
        <div class="text-robotics">
          <h1>Кружок робототехники</h1>
          <p>
            Также в нашей школе проходят занятия по РОБОТОТЕХНИКЕ! 
            Ребята учатся собирать и управлять конструктором. 
            Придумывать новые модели, находить способы решения 
            трудных задач и развивать логическое мышление
          </p>
          <button class="btn-robotics">Узнать больше</button>
        </div>
       </div>
      </div>
    </section>
</template>

<style>

.robotics-club {
  padding: 80px 0;
}

.image-robotics {
  display: flex;
  justify-content: space-between;
  gap: 30px;
}

.robot {
  max-width: 550px;
  height: 550px;
  object-fit: contain;
}

.text-robotics {
  max-width: 660px;
  text-align: center;
}

.text-robotics h1 {
  font-size: 50px;
  color: #3F1B62;
  margin-bottom: 20px;
  text-align: center;
}

.text-robotics p {
  font-size: 30px;
  line-height: 1.5;
  text-align: center;
}

.btn-robotics {
  background: #6f239c;
  color: white;
  border: none;
  border-radius: 40px;
  padding: 16px 40px;
  font-size: 16px;
  cursor: pointer;
  align-self: center;
  font-weight: 700;
}

.btn-robotics:hover {
  opacity: 0.85;
}

</style>