<template>
      <div class="hero">
      <div class="hero-content">
          <h3>ВАШ НАДЕЖНЫЙ ПАРТНЕР В АВТОМАТИЗАЦИИ</h3>
          <h1>ПЕРВЫЙ РОССИЙСКИЙ
            ПРОИЗВОДИТЕЛЬ</h1>
          <p>Умное устройство с тактильной обратной связью для управления сложными техническими системами</p>
      </div>
  </div>

  <!-- Второй блок -->
  <div class="features">
      <h2>ДЛЯ КОГО</h2>
      <div class="feature-items">
          <div class="feature-item">
              <img src="/img/zavod1.png" alt="Service 1">
              <h3>ДЛЯ ПРОМЫШЛЕННЫХ ПРЕДПРИЯТИЙ</h3>
              <p>Компании, занимающиеся производством в различных отраслях, таких как автомобильная, электронная, машиностроительная и другие, которые используют сложные технические системы и механизмы.</p>
          </div>
          <div class="feature-item">
              <img src="/img/zavod2.png" alt="Service 2">
              <h3>ДЛЯ РОБОТОТЕХНИЧЕСКИХ ПРЕДПРИЯТИЙ</h3>
              <p>Организации, разрабатывающие и производящие роботов и автоматизированные системы для применения в производственных линиях, складах и других областях.</p>
          </div>
          <div class="feature-item">
              <img src="/img/zavod3.png" alt="Service 3">
              <h3>ДЛЯ ПРОИЗВОДИТЕЛЕЙ ПРОМЫШЛЕННОГО ОБОРУДОВАНИЯ</h3>
              <p>Компании, которые специализируются на разработке и производстве оборудования для управления техническими системами, таких как станки с числовым программным управлением, промышленные роботы и другое оборудование.</p>
          </div>
          <div class="feature-item">
              <img src="/img/zavod4.png" alt="Service 4">
              <h3>ДЛЯ КОМПАНИЙ АДДИТИВНОГО ПРОИЗВОДСТВА</h3>
              <p>Предприятия, занимающиеся 3D-печатью и аддитивным производством, которые нуждаются в управлении процессами печати и контроле качества изделий.</p>
          </div>
      </div>
  </div>
  <!-- МОСТ -->
  <div class="cta-section">
  <h2>ЗАБУДЬТЕ О РУЧНОМ УПРАВЛЕНИИ, ПОРА АВТОМАТИЗИРОВАТЬ</h2>
  <a href="#section1" class="button">ХОЧУ!</a>
  </div>
  <!-- Третий блок -->
  <div class="grid-section">
      <h2 class="grid-title">ОСНОВНЫЕ ПРЕИМУЩЕСТВА</h2>
      <div class="grid-items">
          <div class="grid-item">
              <img src="/img/text1.png" alt="">
              <h3>ПОВЫШЕННАЯ ПРОИЗВОДИТЕЛЬНОСТЬ</h3>
              <p>Благодаря оптимизированному дизайну и эффективной технологии управления, наше устройство способствует повышению производительности технических систем и сокращению времени настройки и перенастройки.</p>
          </div>
          <div class="grid-item">
              <img src="/img/text2.png" alt="">
              <h3>НАДЕЖНОСТЬ И ПРОЧНОСТЬ</h3>
              <p>Конструктивные особенности устройства обеспечивают его долговечность и надежную работу даже в условиях повышенной нагрузки. Это гарантирует стабильное функционирование системы управления на протяжении всего срока службы.</p>
          </div>
          <div class="grid-item">
              <img src="/img/text3.png" alt="">
              <h3>КАЧЕСТВО</h3>
              <p>Выбранное техническое решение представляет собой сбалансированную комбинацию функциональности, надежности и доступности, что делает его привлекательным выбором для широкого круга потенциальных потребителей.</p>
          </div>
          <div class="grid-item">
              <img src="/img/text4.png" alt="">
              <h3>УДОБСТВО В ИСПОЛЬЗОВАНИИ</h3>
              <p>Разработанное устройство обладает интуитивно понятным пользовательским интерфейсом и тактильным откликом, что значительно упрощает процесс взаимодействия оператора с системой управления. Это снижает вероятность ошибок и повышает эффективность работы.</p>
          </div>
          <div class="grid-item">
              <img src="/img/text5.png" alt="">
              <h3>ЭКОНОМИЧНОСТЬ</h3>
              <p>Проектирование устройства учитывает доступность и дешевизну материалов, что способствует снижению себестоимости производства. Это позволяет создать конкурентоспособный продукт на рынке.</p>
          </div>
          <div class="grid-item">
              <img src="/img/text6.png" alt="">
              <h3>ГИБКОСТЬ И УНИВЕРСАЛЬНОСТЬ</h3>
              <p>Устройство предназначено для интеграции с различными техническими системами, что делает его универсальным решением для широкого спектра применений. Оно может быть успешно использовано как в производственных, так и в промышленных сферах.</p>
          </div>
      </div>
  </div>

  <!-- Четвертый блок -->
  <div class="about-section">
      <div class="about-image">
          <img src="/img/Render_1_(1)-transformed 1.png" alt="About Us">
      </div>
      <div class="about-content">
          <h2>ТОЧНОСТЬ, СКОРОСТЬ, ЭФФЕКТИВНОСТЬ</h2>
          <p>Наше техническое предложение включает разработку умного устройства с тактильной обратной связью, которое оборудовано сенсорным экраном и интерактивными элементами управления. Инновационность заключается в интеграции передовых технологий обратной связи, которые повышают чувствительность и точность реакции устройства на команды пользователя, улучшая тем самым интерактивность и функциональность в процессах управления сложными системами.</p>
      </div>
  </div>
  <!-- МОСТ -->
  <div class="cta-section">
      <h2>МЫ ВАШ ПУТЬ К ЭФФЕКТИВНОЙ РАБОТЕ</h2>
      <a href="#section1" class="button">ХОЧУ!</a>
  </div>
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
