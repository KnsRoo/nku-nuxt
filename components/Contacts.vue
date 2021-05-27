<template>
  <section>
  <h2 class="title">КОНТАКТЫ</h2>
  <div class="contacts">
    <div class="contacts__content">
      <div class="contacts__contacts">
        <div class="contacts__item">
          Телефон:<a class="contacts__link" href="tel:+79164441159">+7-916-444-11-59</a>
        </div>
        <div class="contacts__item">
          E-mail:<a class="contacts__link" href="mailto:info@nku.su">info@nku.su</a>
        </div>
        <div class="contacts__item">
          Адрес: г. Москва, ул. Маршала Захарова, д. 23
        </div>
      </div>

      <h3>Реквизиты</h3>
      <div>
        ООО «НКУ»<br>
        Юр. адрес: 115582, г. Москва, б-р Ореховый, д. 14, корп. 1, 374<br>
        ОГРН: 1187746358238<br>
        ИНН: 7724435224<br>
        КПП: 772401001<br>
        Банк: АО "ТИНЬКОФФ БАНК"<br>
        БИК: 044525974<br>
        Р/с: 40702810510000316785<br>
        К/с: 30101810145250000974<br>
      </div>
    </div>
    <div class="contacts__map">
      <iframe width="100%" height="100%"
              src="https://yandex.ru/map-widget/v1/?um=constructor%3Ac087a7b8e5132591841130cfd525f51f4e88ce3b2872094f069a0761272c84ca"></iframe>
    </div>
  </div>
  </section>
</template>

<script>
export default {
  name: "Contacts"
}
</script>

<style>

.contacts {
  display: flex;
  overflow: hidden;
  margin-top: 20px;
}

.contacts__content {
  display: flex;
  overflow: hidden;
  flex-direction: column;
  line-height: 1.5;
  max-width: 300px;
}

.contacts__contacts {
  display: flex;
  overflow: hidden;
  font-size: 1.5rem;
  margin-bottom: 30px;
  flex-direction: column;
}

.contacts__item {
  display: flex;
  overflow: hidden;
}

.contacts__link {
  color: #000;
  text-decoration: none;
  margin-left: 6px;
}

.contacts__map {
  margin-left: 20px;
  flex-grow: 1;
}

@media (max-width: 576px) {
  .contacts {
    flex-direction: column;
  }

  .contacts__map {
    margin-left: 0;
    margin-top: 30px;
    height: 300px;
  }
}
</style>