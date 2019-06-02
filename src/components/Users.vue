<template>
    <div class="users">
      <ul>
        <li v-for="user in users">
          {{user}}
        </li>
      </ul>
    </div>
</template>

<script>
    export default {
        name: "Users",
      data(){
          return{
            users:['H','B','E']
          }
      }
    }
</script>

<style scoped>

</style>
