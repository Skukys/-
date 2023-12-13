<template>
  <div class="content">
    <div class="content-form">
      <div class="content-form__item small">
        <div class="content-form__item-title">Откуда</div>
        <base-select :class="[validate.firstSity ? 'error' : '']" :options="sities" v-model="formData.firstSity"></base-select>
      </div>
      <div class="content-form__item small">
        <div class="content-form__item-title">Куда</div>
        <base-select :class="[validate.secondSity ? 'error' : '']" :options="sities" v-model="formData.secondSity"></base-select>
      </div>
      <div class="content-form__item big">
        <div class="content-form__item-title">Даты</div>
        <base-date :class="[validate.date ? 'error' : '']" v-model="formData.date"></base-date>
      </div>
      <button class="content-form__button" @click="search">
        Найти
      </button>
    </div>
  </div>
</template>

<script>
import baseSelect from "../components/baseSelect.vue"
import baseDate from "../components/baseDate.vue"

export default {
  name: "FormPage",
  components: {
    baseSelect, baseDate
  },
  data(){
    return {
      sities: [
        'Atlanta',
        'Boston',
        'Chicago',
        'Dallas',
        'Detroit',
        'Honolulu',
        'Houston',
        'Las Vegas',
        'New York City',
      ],
      formData: {
        firstSity: null,
        secondSity: null,
        date: null,
      },
      validate: {
        firstSity: false,
        secondSity: false,
        date: false,
      }
    }
  },
  watch: {
    'formData.firstSity': function (){this.validate.firstSity = !this.formData.firstSity},
    'formData.secondSity': function (){this.validate.secondSity = !this.formData.secondSity},
    'formData.date': function (){this.validate.date = !this.formData.date},
  },
  methods: {
    search(){
      this.checkValidate()
      console.log(this.formData)
    },
    checkValidate(){
      if(!this.formData.firstSity) this.validate.firstSity = true
      if(!this.formData.secondSity) this.validate.secondSity = true
      if(!this.formData.date) this.validate.date = true
    }
  },
}
</script>

<style scoped>

</style>