# Vue Infinite Scroll Component

![NPM License](https://img.shields.io/npm/l/vue-infinite-scroll-component)

**Lightweight** infinite scroll component for [Vue](https://vuejs.org/) **< 5k** 😎 <br>

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
