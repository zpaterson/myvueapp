<template>
  <div class="test">
      <input type="text" v-model="title">
      <br />
     <h1>{{title}}</h1>
     <!-- <span v-html="title"></span> -->
     <p v-if="showName">{{user.firstName}}</p>
     <p v-else>You don't have a name</p>
     <!-- <p v-text="user.lastName"></p> -->
     <ul>
       <li v-for="item in items" v-bind:key="item">{{item.title}}</li>
     </ul>
  </div>
</template>

<script>
    export default {
       name: 'test',
       data() {
          return {
            title: 'Hello World',
            // title: '<h1>Hello Worlds</h1>',
            user: {
              firstName: 'Zaire',
              lastName: 'Paterson'
            },
            showName: true,
            items: [
              {title: 'Item One'},
              {title: 'Item Two'},
              {title: 'Item Three'},
            ]
          }
       } 
    }
</script>

<style scoped>

</style>

