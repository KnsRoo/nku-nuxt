<template>
  <div class="request">
    <h2 class="request__header">
      Оставить заявку
    </h2>

    <div class="request__content">
      <div class="label">
        <label class="label__name">Телефон</label>
        <input class="label__input" placeholder="Введите номер телефона"/>
        <span class="label__error">Необходимо указать номер телефона</span>
      </div>
    </div>

    <div class="request__footer">
      <button class="button">Отправить</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Request"
}
</script>

<style>
.request {
  display: flex;
  overflow: hidden;
  flex-flow: column;
  align-self: center;
  margin-top: 50px;
  width: 100%;
  max-width: 500px;
}

.request__header {
  display: flex;
  overflow: hidden;
  background-color: #3e4757;
  padding: 20px 10px;
  border-top-left-radius: 10px;
  border-top-right-radius: 10px;
  text-align: center;
  color: white;
  font-size: 1.5rem;
}

.request__content {
  display: flex;
  overflow: hidden;
  padding: 30px 10px;
  border-left: 1px solid #eef2e7;
  border-right: 1px solid #eef2e7;
}

.label {
  display: flex;
  overflow: hidden;
}

.request__footer {
  display: flex;
  overflow: hidden;
  padding: 10px 10px;
  border-bottom-left-radius: 10px;
  border-bottom-right-radius: 10px;
  border: 1px solid #eef2e7;
}
</style>