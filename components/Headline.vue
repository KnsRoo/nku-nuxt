<template>
  <section>
  <h1 class="headline__title">{{ title }}</h1>
  <div class="headline">
    <img
      class="headline__image"
      :src="'/img/' + image"
      :alt="title"
    />

    <div class="headline__description">
      <h2 class="headline__header">
        {{ benefit }}
      </h2>
      <ul class="headline__advantages">
        <li
          v-for="(advantage, idx) in advantages"
          :key="idx"
          class="headline__advantage"
        >
          {{ advantage }}
        </li>
      </ul>
    </div>
  </div>
  </section>
</template>

<script>
export default {
  name: "Headline",
  props: {
    title: String,
    image: String,
    benefit: String,
    advantages: Array,
  },
};
</script>

<style>
.headline {
  display: flex;
  overflow: hidden;
  margin-top: 50px;
  justify-content: center;
  align-items: center;
}

.headline__title {
  margin: 2rem auto 0 auto;
  font-size: 2rem;
  font-weight: bold;
  text-align: center;
  max-width: 700px;
}

.headline__image {
  max-width: 300px;
  padding-right: 50px;
}

.headline__description {
  display: flex;
  overflow: hidden;
  max-width: 500px;
  flex-direction: column;
}

.headline__header {
  font-size: 1.5rem;
  font-weight: bold;
}

.headline__advantages {
  margin-top: 20px;
  font-size: 1.25rem;
  margin-left: 20px;
}

.headline__advantage {
  margin-top: 5px;
}

@media (max-width: 768px) {
  .headline {
    flex-direction: column;
  }

  .headline__image {
    padding-right: 0;
  }

  .headline__description {
    margin-top: 50px;
  }
}
</style>