<template>

  <select name="genere" 
  id="genere"
  v-model="inputText"
  @change="$emit('sendSearch',inputText)"
  >
    <option value="metal">Metal</option>
    <option value="jazz">Jazz</option>
    <option value="pop">Pop</option>
    <option value="rock">Rock</option>
  </select>

</template>

<script>
export default {
  nome: "Selezione",

  data(){
    return {
      inputText :'',
    }
  },

}

</script>

<style>

#genere{
  margin-right: 25px;
  background-color: #50d850;
  color: black;
  border: none;
  border-radius: 5px;
  padding: 10px 5px;
}

</style>