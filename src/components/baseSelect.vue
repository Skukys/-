<template>
  <div
      class="custom-select"
      :tabindex="tabindex"
  >
    <div
        class="selected"
        :class="{open: open}"
        @click="open = !open"
    >
      <img src="../assets/icons/location.svg"><p>{{ selected }}</p>
    </div>
    <div
        class="items"
        :class="{selectHide: !open}"
    >
      <input class="custom-select__search" placeholder="Filter" v-model="filterValue">
      <div
          class="item"
          v-for="(option, i) of filteredOptions"
          :key="i"
          @click="select(option)"
      >
        {{ option }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "baseSelect",
  props:{
    modelValue: {
      default: null,
    },
    options:{
      type: Array,
      required: true
    },
    tabindex:{
      type: Number,
      required: false,
      default: 0
    }
  },
  data() {
    return {
      selected: 'Выберите город',
      open: false,
      filterValue: null,
      filteredOptions: []
    };
  },
  watch: {
    filterValue(){
      this.filter()
    }
  },
  methods: {
    select(option){
      this.selected = option
      this.open = false
      this.$emit('update:modelValue', option)
    },
    filter(){
      if(this.filterValue) {
        this.filteredOptions = this.filteredOptions.filter(el => el.includes(this.filterValue))
      } else {
        this.filteredOptions = this.options
      }
    }
  },
  mounted(){
    this.filteredOptions = this.options
  }
}
</script>

<style scoped>

</style>