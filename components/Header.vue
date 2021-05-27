<template>
  <header class="header">
    <div class="header__container">
      <a class="header__company" href="/">NKU</a>
      <div class="header__right">
        <a class="header__email" href="mailto:info@nku.su">info@nku.su</a>
        <a class="header__phone" href="tel:+79164441159">+7-916-444-11-59</a>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style>
.header {
  padding: 2px 0;
  background-color: #026aa7;
  justify-content: center;
}

.header__container {
  display: flex;
  overflow: hidden;
  justify-content: space-between;
  align-items: center;
  width: 1120px;
  padding: 0 10px;
}

.header__company {
  color: #fff;
  font-size: 3rem;
  text-decoration: none;
}

.header__company:hover {
  color: #fff;
  text-decoration: none;

}

.header__right {
  display: flex;
  overflow: hidden;
  align-items: center;
}

.header__email {
  color: #fff;
  font-size: 1.5rem;
  text-decoration: none;
}

.header__phone {
  color: #fff;
  font-size: 1.75rem;
  margin-left: 40px;
  text-decoration: none;
}

@media (max-width: 576px) {
  .header__container {
    flex-direction: column;
  }

  .header__right {
    flex-direction: column;
  }

  .header__email {
    margin-top: 10px;
  }

  .header__phone {
    margin-left: 0;
    margin-top: 10px;
  }
}
</style>