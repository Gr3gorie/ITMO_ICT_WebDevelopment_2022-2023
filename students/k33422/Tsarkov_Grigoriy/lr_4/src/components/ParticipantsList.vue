<template>
<div>
  <v-card
      elevation="2"
      outlined
      class="my-2"
    >
    <v-card-text>
 <div  v-for="participant in participants" :key="participant.id"> 
   <div><strong>Никнейм:</strong> {{ participant.name }}</div>
   <div><strong>Фандом:</strong> {{ participant.fandom }}</div>
   <div><strong>Возраст:</strong> {{ participant.age }}</div>
   <div><strong>Персонаж:</strong> {{ participant.character }}</div>
   <div><strong>Клуб:</strong> {{ participant.club }}</div><br>
 </div>
    </v-card-text>
  </v-card>
</div>
</template>

<script>
export default {
 props: { 
   participants: {
     type: Array,
     required: true
   }
 }
}
</script>

<style scoped>

</style>