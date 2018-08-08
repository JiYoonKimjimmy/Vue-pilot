<template>
  <div class="index">
    <select v-model="selected">
      <option v-for="option in options" v-bind:value="option.value">
        {{ option.text }}
      </option>
    </select>
    <span>선택함: {{ selected }}</span>
  </div>
</template>

<script>
export default {
  name: 'Index',
  data () {
    return {
      selected: 'A',
      options: [
        {text:'one', value:'A'},
        {text:'two', value:'B'},
        {text:'three', value:'C'}
      ]
    }
  }
}
</script>
