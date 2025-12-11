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
            <form class="banner-form" @submit.prevent="sendForm">
                <input v-model="phone" type="tel" placeholder="+7 999-999-99-99" required />
                <input v-model="name" type="text" placeholder="Имя" required />
                <button type="submit">{{ loading ? "Отправка..." : "Заказать звонок" }}</button>
                <p v-if="status" class="status">{{ status }}</p>
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

<script>
export default {
    data() {
        return {
            phone: "",
            name: "",
            loading: false,
            status: ""
        };
    },
    methods: {
        async sendForm() {
            this.loading = true;
            this.status = "";
            const token = "8544309188:AAGLQ0JguNHCZD_ca-fExaoVo4Dh6eip3JE";
            const chat_id = "1056711179";
            const text = `📩 Новая заявка:
            📞 Телефон: ${this.phone}
            👤 Имя: ${this.name}`;
            try {
        const res = await fetch(`https://api.telegram.org/bot${token}/sendMessage?chat_id=${chat_id}&text=${encodeURIComponent(text)}`);
        const data = await res.json();
        if (data.ok) {
            this.status = "✔️ Заявка отправлена!";
            this.phone = "";this.name = "";
        } else {
            this.status = "Ошибка отправки";
        }
    } catch (e) {
        this.status = "Ошибка соединения";
    }
    this.loading = false;
    }
}
};
</script>

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
.banner-form button:hover {
    background-color:#ff007f;
}
.banner-image {
    max-width: 560px;
}
</style>