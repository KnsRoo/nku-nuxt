<template>
  <Nuxt />
</template>

<style>
body {
  font-family: Georgia, sans-serif;
  line-height: 1.25;
}

header, footer, main, label, iframe {
  display: flex;
  overflow: hidden;
}

* {
  padding: 0;
  margin: 0;
}

input, iframe {
  border: none;
  outline: none;
  background-color: inherit;
}

h1 {
  font-size: 2.5rem;
}

h2 {
  font-size: 2rem;
}

h3 {
  font-size: 1.75rem;
}

h4 {
  font-size: 1.5rem;
}

h5 {
  font-size: 1.25rem;
}

h6 {
  font-size: 1rem;
}

.button {
  font-size: 1.25rem;
  padding: 16px 5px;
  background-color: #ffdd2d;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  box-sizing: content-box;
  flex-grow: 1;
}

.button:focus {
  outline: none;
}

.label {
  flex-flow: column;
  padding: 10px;
  border-radius: 10px;
  background-color: #eef2f7;
  flex-grow: 1;
}

.label__name {
  color: #9299a2;
  font-size: 1rem;
}

.label__input {
  font-size: 1.25rem;
  margin-top: 8px;
}

.label__error {
  display: none;
  color: #dd5656;
  font-size: 1rem;
}

.label_is-error {
  display: flex;
}

.title {
  margin: 2rem auto 0 auto;
  font-weight: bold;
  text-align: center;
  max-width: 700px;
}
</style>
