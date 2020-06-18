<template>
  <div>
    <ol class="tab">
      <li v-for="(item, index) in items" :key="index" class="tab-list">
        <router-link v-bind:to="item.path">
          {{ item.title }}
        </router-link>
      </li>
    </ol>
  </div>
</template>

<script>
export default {
  name: "TabMenu",
  data(){
    return {
      items: [
        {title: "top", path: "/"},
        {title: "profile", path: "/profile"},
        {title: "skill", path: "/skill"},
        {title: "contact", path: "/contact"}
      ]
    }
  }
}
</script>

<style>
body {
  margin: 0;
}

.tab{
  list-style: none;
  display: flex;
  background-color:skyblue;
  margin: 0;
  width:100%;
}

.tab-list{
  padding: 15px;
}
</style>