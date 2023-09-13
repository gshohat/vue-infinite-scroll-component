# Vue Infinite Scroll Component

![NPM License](https://img.shields.io/npm/l/vue-infinite-scroll-component)

**Lightweight** infinite scroll component for [Vue](https://vuejs.org/) **< 5k** 😎 <br>

![infinite-scroll](https://private-user-images.githubusercontent.com/91323932/267593435-aba9d3c1-7c16-4633-bb0c-a55a6781ca09.gif?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTQ1OTUxOTgsIm5iZiI6MTY5NDU5NDg5OCwicGF0aCI6Ii85MTMyMzkzMi8yNjc1OTM0MzUtYWJhOWQzYzEtN2MxNi00NjMzLWJiMGMtYTU1YTY3ODFjYTA5LmdpZj9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFJV05KWUFYNENTVkVINTNBJTJGMjAyMzA5MTMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjMwOTEzVDA4NDgxOFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTgwMDlhYzM3YWMyNzA4ZTdkNjU1ZmNhNmVkN2NkMzkyZmQ2ZTE0MjY0YzUwYmQzOTkzOGMwMmJhZWJmY2JiZDMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.v_-iW0UhaobXvXONdUZ55F4tak9wnjRB6HrhHsCPPKE)

## Usage

`npm i vue-infinite-scroll-component`

```
<script setup>
import InfiniteScrollComponent from 'vue-infinite-scroll-component';
import 'vue-infinite-scroll-component/dist/style.css';

const options = {
  fetchData,
};

async function fetchData() {
  const res = await fetch('https://.../texts/works.json');
  return await res.json();
}
</script>


<template>
  <Suspense>
    <InfiniteScrollComponent :options="options" v-slot="slotProps">

      <!-- your component -->
      <ul>
        <li v-for="item in slotProps.items">
          {{item.title}}
        </li>
      </ul>

    </InfiniteScrollComponent>
  </Suspense>
</template
```


## Contact
Feel free to ping me 💫
<br>
connect@giladshohat.com

[giladshohat.com](https://giladshohat.com)
