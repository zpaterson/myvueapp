<template>
  <div class="test">
     <h1>{{title}}</h1>
     <!-- <span v-html="title"></span> -->
     <p v-if="showName">{{user.firstName}}</p>
     <p v-else>You don't have a name</p>
     <!-- <p v-text="user.lastName"></p> -->
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
            showName: true
          }
       } 
    }
</script>

<style scoped>

</style>

