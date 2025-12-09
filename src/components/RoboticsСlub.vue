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
            трудных задач и развивать логическое мышление.
          </p>
          <button class="robot-btn">Узнать больше</button>
        </div>
       </div>
      </div>
    </section>
</template>

<style>

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.robotics-club {
  padding: 80px 0;
}

.image {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 40px;
}

.robot {
  max-width: 450px;
  width: 100%;
  object-fit: contain;
}

.text {
  
}

.text h1 {
  font-size: 48px;
  font-weight: 700;
  color: #3F1B62;
  margin-bottom: 20px;
}

.robot-text p {
  font-size: 4px;
  line-height: 1.4;
  margin-bottom: 30px;
}

.robot-btn {
  background: #6f239c;
  color: white;
  border: none;
  border-radius: 40px;
  padding: 16px 40px;
  font-size: 20px;
  cursor: pointer;
  transition: 0.2s;
}

.robot-btn:hover {
  opacity: 0.85;
}
</style>