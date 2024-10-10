<template>

  <div class="feedback-container">
  <!-- Левая часть: Форма обратной связи -->
  <a id="section1"></a>
  <div class="feedback-form-container">
  <form @submit.prevent="submitForm">
    <h2>Оставьте заявку</h2>
    <input type="text" name="name" placeholder="Введите имя" v-model="name"/>
    <input type="text" name="lastname" placeholder="Введите фамилию" v-model="lastname"/>
    <input type="text" name="lastlastname" placeholder="Введите Отчество" v-model="lastlastname"/>
    <input type="email" name="email" placeholder="Email" v-model="email"/>
    <input type="text" name="message" placeholder="комментарий" v-model="message"/>
    <button type="submit">Отправить</button>
  </form>
  </div>

  <!-- Правая часть: Информация -->

  <div class="contact-info-container">
      <div>
          <h2>Свяжитесь с нами</h2>
          <p>Мы всегда готовы ответить на ваши вопросы и помочь с любыми задачами.</p>
      </div>
      <div class="contact-icons">
          <div>
              <img src="/img/icons10.png" alt="Phone Icon">
              <p>+7 (919) 445-32-54 </p>
          </div>
          <div>
              <img src="/img/icons11.png" alt="Email Icon">
              <p>viskunovdmitrij1@gmail.com</p>
          </div>
      </div>
  </div>
</div>

</template>
<script>
const WEB3FORMS_ACCESS_KEY = "5fee4d3d-caad-48c7-8885-ea9f433b1957";

export default {
data() {
  return {
    error:"",  
    name: "",
    lastname: "",
    lastlastname: "",
    email: "",
    message: "",
  };
},
methods: {
  sendData(){
      if(this.name == ''){
          this.error = 'Имя не введено';
          return;
      }else if(this.lastname == ''){
          this.error = 'Фамилия не введена';
          return;
      }else if (this.email == ''){
          this.error = 'Email не введен';
          return;
      }
      this.error='';  
  },
  async submitForm() {
    const response = await fetch("https://api.web3forms.com/submit", {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
        Accept: "application/json",
      },
      body: JSON.stringify({
        access_key: WEB3FORMS_ACCESS_KEY,
        name: this.name,
        lastname: this.lastname,
        lastlastname: this.lastlastname,
        email: this.email,
        message: this.message,
      }),
    });
    const result = await response.json();
    if (result.success) {
      console.log(result);
    }
  },
},
};
</script>

<style scoped>
input{
  display: block;
  margin-bottom: 10px;
  border-radius: 3px;
  border: 1px solid silver;
  outline: none;
  padding-right: 70%;
  padding-left: 5%;
  padding-top: 5%;
  padding-bottom: 5%;
  background: #fafafa;
  color: #333;
}
input:hover{
  transform: scale(1.01);
}
button{
  border: 0;
  border-radius: 5px;
  outline: none;
  padding: 10px 15px;
  background: #f69e1a;
  color: #000;
  font-weight: bold;
  cursor: pointer;
  transition: transform 500ms ease;
}
button:hover{
  transform: translateY(-5px);
}
</style>
