<template>
  <div class="custom-date" :tabindex="tabindex" @blur="open = false">
    <div class="custom-date__top" :class="{open: open}" @click="open = true">
      <p class="custom-date__top-date">
        <svg width="12" height="13" viewBox="0 0 12 13" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M11.4707 2.61278C11.389 2.53206 11.2909 2.46794 11.1822 2.42433C11.0735 2.38071 10.9565 2.35852 10.8384 2.3591H9.93274V1.71778C9.93482 1.57713 9.90643 1.43756 9.84934 1.3077C9.79225 1.17784 9.70767 1.06043 9.60081 0.96271C9.49754 0.861661 9.37352 0.781709 9.23637 0.727783C9.09922 0.673856 8.95186 0.647098 8.80338 0.649158H8.3521C8.20356 0.647195 8.05617 0.674071 7.91902 0.728127C7.78187 0.782183 7.65787 0.862274 7.55467 0.963458C7.44777 1.06115 7.36317 1.17855 7.30607 1.30842C7.24898 1.43829 7.22062 1.57787 7.22274 1.71853V2.35985H4.51274V1.71778C4.51481 1.57713 4.48643 1.43756 4.42934 1.3077C4.37225 1.17784 4.28766 1.06043 4.1808 0.96271C4.07763 0.861753 3.95373 0.781855 3.81672 0.727932C3.67972 0.674009 3.53251 0.647201 3.38416 0.649158H2.93289C2.78434 0.647195 2.63695 0.674071 2.4998 0.728127C2.36265 0.782183 2.23865 0.862274 2.13545 0.963458C2.02859 1.06117 1.94401 1.17858 1.88692 1.30845C1.82983 1.43831 1.80145 1.57787 1.80352 1.71853V2.35985H0.900184C0.782128 2.35927 0.665186 2.38146 0.556485 2.42508C0.447783 2.46869 0.349602 2.53281 0.267929 2.61353C0.182682 2.69087 0.114961 2.78383 0.0688993 2.88676C0.0228373 2.98968 -0.000601975 3.10041 1.05193e-05 3.2122V11.7664C0.00305796 11.9919 0.0987552 12.2074 0.266805 12.3672C0.434854 12.5271 0.662039 12.6186 0.900184 12.6225H10.8353C11.0739 12.6194 11.3017 12.5283 11.4704 12.3685C11.6391 12.2088 11.7354 11.993 11.7386 11.7671V3.21444C11.7397 3.10215 11.7164 2.99085 11.6704 2.88738C11.6243 2.78391 11.5563 2.69046 11.4707 2.61278ZM2.93526 11.7664H0.900184V9.84242H2.9321L2.93526 11.7664ZM2.93526 9.41438H0.900184V7.27639H2.9321L2.93526 9.41438ZM2.93526 6.84835H0.900184V4.92438H2.9321L2.93526 6.84835ZM2.77719 3.79141C2.75581 3.77212 2.73882 3.74889 2.72726 3.72315C2.71571 3.69741 2.70984 3.66971 2.71002 3.64174V1.71778C2.71083 1.66126 2.73491 1.60727 2.77712 1.5673C2.81934 1.52733 2.87635 1.50453 2.93605 1.50375H3.38416C3.44385 1.50453 3.50087 1.52733 3.54308 1.5673C3.5853 1.60727 3.60937 1.66126 3.61019 1.71778V3.64249C3.60937 3.69901 3.5853 3.753 3.54308 3.79297C3.50087 3.83294 3.44385 3.85574 3.38416 3.85651H2.93289C2.90304 3.85674 2.87345 3.85115 2.84599 3.84007C2.81852 3.829 2.79376 3.81269 2.77324 3.79215L2.77719 3.79141ZM5.64526 11.7656H3.38416V9.84242H5.6421L5.64526 11.7656ZM5.64526 9.41363H3.38416V7.27639H5.6421L5.64526 9.41363ZM5.64526 6.8476H3.38416V4.92438H5.6421L5.64526 6.8476ZM8.35527 11.7649H6.09337V9.84242H8.35131L8.35527 11.7649ZM8.35527 9.41288H6.09337V7.27639H8.35131L8.35527 9.41288ZM8.35527 6.84685H6.09337V4.92438H8.35131L8.35527 6.84685ZM8.1972 3.78991C8.17543 3.77118 8.15789 3.74845 8.14566 3.72311C8.13344 3.69777 8.12677 3.67034 8.12607 3.64249V1.71778C8.12669 1.6612 8.1507 1.6071 8.19296 1.56709C8.23521 1.52707 8.29235 1.50434 8.3521 1.50375H8.80338C8.86313 1.50434 8.92027 1.52707 8.96252 1.56709C9.00478 1.6071 9.02879 1.6612 9.02941 1.71778V3.64249C9.02879 3.69907 9.00478 3.75317 8.96252 3.79318C8.92027 3.83319 8.86313 3.85593 8.80338 3.85651H8.3521C8.32225 3.85679 8.29265 3.85121 8.26518 3.84014C8.2377 3.82906 8.21295 3.81272 8.19246 3.79215L8.1972 3.78991ZM10.84 11.7641H8.80338V9.84242H10.8353L10.84 11.7641ZM10.84 9.41213H8.80338V7.27639H10.8353L10.84 9.41213ZM10.84 6.8461H8.80338V4.92438H10.8353L10.84 6.8461Z" fill="#333333"/>
        </svg>
        {{ getFirstDate }}
      </p>
      <span>
        <svg width="22" height="2" viewBox="0 0 22 2" fill="none" xmlns="http://www.w3.org/2000/svg">
          <line x1="0.73877" y1="1.2165" x2="21.1388" y2="1.2165" stroke="#BDBDBD" stroke-width="0.838476"/>
        </svg>
      </span>
      <p class="custom-date__top-date">
        <svg width="12" height="13" viewBox="0 0 12 13" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M11.4707 2.61278C11.389 2.53206 11.2909 2.46794 11.1822 2.42433C11.0735 2.38071 10.9565 2.35852 10.8384 2.3591H9.93274V1.71778C9.93482 1.57713 9.90643 1.43756 9.84934 1.3077C9.79225 1.17784 9.70767 1.06043 9.60081 0.96271C9.49754 0.861661 9.37352 0.781709 9.23637 0.727783C9.09922 0.673856 8.95186 0.647098 8.80338 0.649158H8.3521C8.20356 0.647195 8.05617 0.674071 7.91902 0.728127C7.78187 0.782183 7.65787 0.862274 7.55467 0.963458C7.44777 1.06115 7.36317 1.17855 7.30607 1.30842C7.24898 1.43829 7.22062 1.57787 7.22274 1.71853V2.35985H4.51274V1.71778C4.51481 1.57713 4.48643 1.43756 4.42934 1.3077C4.37225 1.17784 4.28766 1.06043 4.1808 0.96271C4.07763 0.861753 3.95373 0.781855 3.81672 0.727932C3.67972 0.674009 3.53251 0.647201 3.38416 0.649158H2.93289C2.78434 0.647195 2.63695 0.674071 2.4998 0.728127C2.36265 0.782183 2.23865 0.862274 2.13545 0.963458C2.02859 1.06117 1.94401 1.17858 1.88692 1.30845C1.82983 1.43831 1.80145 1.57787 1.80352 1.71853V2.35985H0.900184C0.782128 2.35927 0.665186 2.38146 0.556485 2.42508C0.447783 2.46869 0.349602 2.53281 0.267929 2.61353C0.182682 2.69087 0.114961 2.78383 0.0688993 2.88676C0.0228373 2.98968 -0.000601975 3.10041 1.05193e-05 3.2122V11.7664C0.00305796 11.9919 0.0987552 12.2074 0.266805 12.3672C0.434854 12.5271 0.662039 12.6186 0.900184 12.6225H10.8353C11.0739 12.6194 11.3017 12.5283 11.4704 12.3685C11.6391 12.2088 11.7354 11.993 11.7386 11.7671V3.21444C11.7397 3.10215 11.7164 2.99085 11.6704 2.88738C11.6243 2.78391 11.5563 2.69046 11.4707 2.61278ZM2.93526 11.7664H0.900184V9.84242H2.9321L2.93526 11.7664ZM2.93526 9.41438H0.900184V7.27639H2.9321L2.93526 9.41438ZM2.93526 6.84835H0.900184V4.92438H2.9321L2.93526 6.84835ZM2.77719 3.79141C2.75581 3.77212 2.73882 3.74889 2.72726 3.72315C2.71571 3.69741 2.70984 3.66971 2.71002 3.64174V1.71778C2.71083 1.66126 2.73491 1.60727 2.77712 1.5673C2.81934 1.52733 2.87635 1.50453 2.93605 1.50375H3.38416C3.44385 1.50453 3.50087 1.52733 3.54308 1.5673C3.5853 1.60727 3.60937 1.66126 3.61019 1.71778V3.64249C3.60937 3.69901 3.5853 3.753 3.54308 3.79297C3.50087 3.83294 3.44385 3.85574 3.38416 3.85651H2.93289C2.90304 3.85674 2.87345 3.85115 2.84599 3.84007C2.81852 3.829 2.79376 3.81269 2.77324 3.79215L2.77719 3.79141ZM5.64526 11.7656H3.38416V9.84242H5.6421L5.64526 11.7656ZM5.64526 9.41363H3.38416V7.27639H5.6421L5.64526 9.41363ZM5.64526 6.8476H3.38416V4.92438H5.6421L5.64526 6.8476ZM8.35527 11.7649H6.09337V9.84242H8.35131L8.35527 11.7649ZM8.35527 9.41288H6.09337V7.27639H8.35131L8.35527 9.41288ZM8.35527 6.84685H6.09337V4.92438H8.35131L8.35527 6.84685ZM8.1972 3.78991C8.17543 3.77118 8.15789 3.74845 8.14566 3.72311C8.13344 3.69777 8.12677 3.67034 8.12607 3.64249V1.71778C8.12669 1.6612 8.1507 1.6071 8.19296 1.56709C8.23521 1.52707 8.29235 1.50434 8.3521 1.50375H8.80338C8.86313 1.50434 8.92027 1.52707 8.96252 1.56709C9.00478 1.6071 9.02879 1.6612 9.02941 1.71778V3.64249C9.02879 3.69907 9.00478 3.75317 8.96252 3.79318C8.92027 3.83319 8.86313 3.85593 8.80338 3.85651H8.3521C8.32225 3.85679 8.29265 3.85121 8.26518 3.84014C8.2377 3.82906 8.21295 3.81272 8.19246 3.79215L8.1972 3.78991ZM10.84 11.7641H8.80338V9.84242H10.8353L10.84 11.7641ZM10.84 9.41213H8.80338V7.27639H10.8353L10.84 9.41213ZM10.84 6.8461H8.80338V4.92438H10.8353L10.84 6.8461Z" fill="#333333"/>
        </svg>
        {{getSecondDate}}
      </p>
    </div>
    <div class="custom-date__content" :class="{selectHide: !open}">
      <div class="custom-date__content-calendars">
        <div class="custom-date__content-calendar">
          <div class="custom-date__content-calendar-top">
            <div class="custom-date__content-calendar-top__arrow" @click="prevMonth(firstCalendar.date)">
              <svg width="7" height="13" viewBox="0 0 7 13" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M5.99981 11.657L1.7998 6.50002L5.99981 1.34302" stroke="#333333" stroke-width="2"
                      stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
            <div class="custom-date__content-calendar-top__mouth">
              {{ firstCalendar.nameMonth }}
            </div>
            <div class="custom-date__content-calendar-top__arrow" @click="nextMonth(firstCalendar.date)">
              <svg width="7" height="13" viewBox="0 0 7 13" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M1 11.657L5.2 6.50002L1 1.34302" stroke="#333333" stroke-width="2" stroke-linecap="round"
                      stroke-linejoin="round"/>
              </svg>
            </div>
          </div>
          <div class="custom-date__content-calendar-content">
            <div class="custom-date__content-calendar-content__days">
              <span>Пн</span>
              <span>Вт</span>
              <span>Ср</span>
              <span>Чт</span>
              <span>Пт</span>
              <span>Сб</span>
              <span>Вс</span>
            </div>
            <div class="custom-date__content-calendar-content__dates">
              <span v-for="(day, id) in firstCalendar.days" :class="[day.status, day.selected ? 'selected' : '']"
                    @click="select(id, firstCalendar)">{{ day.title }}</span>
            </div>
          </div>
        </div>
        <div class="custom-date__content-calendar">
          <div class="custom-date__content-calendar-top">
            <div class="custom-date__content-calendar-top__arrow" @click="prevMonth(secondCalendar.date, false)">
              <svg width="7" height="13" viewBox="0 0 7 13" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M5.99981 11.657L1.7998 6.50002L5.99981 1.34302" stroke="#333333" stroke-width="2"
                      stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
            <div class="custom-date__content-calendar-top__mouth">
              {{ secondCalendar.nameMonth }}
            </div>
            <div class="custom-date__content-calendar-top__arrow" @click="nextMonth(secondCalendar.date, false)">
              <svg width="7" height="13" viewBox="0 0 7 13" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M1 11.657L5.2 6.50002L1 1.34302" stroke="#333333" stroke-width="2" stroke-linecap="round"
                      stroke-linejoin="round"/>
              </svg>
            </div>
          </div>
          <div class="custom-date__content-calendar-content">
            <div class="custom-date__content-calendar-content__days">
              <span>Пн</span>
              <span>Вт</span>
              <span>Ср</span>
              <span>Чт</span>
              <span>Пт</span>
              <span>Сб</span>
              <span>Вс</span>
            </div>
            <div class="custom-date__content-calendar-content__dates">
              <span v-for="(day, id) in secondCalendar.days"
                    :class="[day.status, day.selected ? 'selected' : '']"
                    @click="select(id, secondCalendar)">{{ day.title }}</span>
            </div>
          </div>
        </div>
      </div>
      <div class="custom-date__content-control flex justify-between items-center">
        <label @click="open = true">
          <input type="checkbox" v-model="multiplySelection" @change="clear">
          <span>Без конечной даты</span>
        </label>
        <button class="content-form__button" @click="open = false">
          Готово
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "baseDate",
  props: {
    tabindex: {
      type: Number,
      required: false,
      default: 0
    },
    modelValue: {
      default: null,
    },
  },
  data() {
    return {
      open: false,
      multiplySelection: false,
      firstCalendar: {
        days: [],
        nameMonth: '',
        date: null
      },
      secondCalendar: {
        days: [],
        nameMonth: '',
        date: null
      },
      currentDate: new Date(),
      days: ['Вс', 'Пн', 'Вт', 'Ср', 'Чт', 'Пт', 'Сб'],
      firstSelect: null,
      secondSelect: null
    }
  },
  computed: {
    getSimpleDateFirst(){
      return new Date(this.firstSelect.calendar.date.getFullYear(), this.firstSelect.calendar.date.getMonth(), this.firstSelect.calendar.days[this.firstSelect.id].title)
    },
    getSimpleDateSecond(){
      return new Date(this.secondSelect.calendar.date.getFullYear(), this.secondSelect.calendar.date.getMonth(), this.secondSelect.calendar.days[this.secondSelect.id].title)
    },
    getFirstDate(){
      if(this.firstSelect) {
        let date = new Date(this.firstSelect.calendar.date.getFullYear(), this.firstSelect.calendar.date.getMonth(), this.firstSelect.calendar.days[this.firstSelect.id].title)
        return this.days[date.getDay()] + " " + this.fixNumber(date.getDate()) + '/' + this.fixNumber(date.getMonth() + 1)
      } else return '----'
    },
    getSecondDate(){
      if(this.secondSelect) {
        let date = new Date(this.secondSelect.calendar.date.getFullYear(), this.secondSelect.calendar.date.getMonth(), this.secondSelect.calendar.days[this.secondSelect.id].title)
        return this.days[date.getDay()] + " " + this.fixNumber(date.getDate()) + '/' + this.fixNumber(date.getMonth() + 1)
      } else return '----'
    }
  },
  methods: {
    fixNumber(num){
      if(num < 10) num = '0' + num
      return num
    },
    nextMonth(date, first = true) {
      let count = first ? 1 : 0
      let start = new Date(date.getFullYear(), date.getMonth() + count, 1)
      this.firstCalendar = this.render(start)
      this.secondCalendar = this.render(new Date(start.getFullYear(), start.getMonth() + 1, 1))
    },
    prevMonth(date, first = true) {
      let count = first ? 1 : 2
      let start = new Date(date.getFullYear(), date.getMonth() - count, 1)
      let testDate = new Date(this.currentDate.getFullYear(), this.currentDate.getMonth(), 1)
      if (start < testDate) return
      this.firstCalendar = this.render(start)
      this.secondCalendar = this.render(new Date(start.getFullYear(), start.getMonth() + 1, 1))
    },
    render(date) {
      let days = []
      let firstDay = new Date(date.getFullYear(), date.getMonth(), 1)
      let lastDayCurrentMonth = new Date(date.getFullYear(), date.getMonth() + 1, 0)
      let testDate = new Date(this.currentDate.getFullYear(), this.currentDate.getMonth(), 1)
      let isCurrentMonth = testDate.getTime() === date.getTime()
      let lastMonth = null


      let checkDate = false
      let startDate = false
      let endDate = false
      if((this.firstSelect && this.secondSelect) || (this.firstSelect && !this.multiplySelection)) checkDate = true
      if(checkDate){
        startDate = new Date(this.firstSelect.calendar.date.getFullYear(), this.firstSelect.calendar.date.getMonth(), this.firstSelect.calendar.days[this.firstSelect.id].title)
        endDate = new Date(this.secondSelect.calendar.date.getFullYear(), this.secondSelect.calendar.date.getMonth(), this.secondSelect.calendar.days[this.secondSelect.id].title)

        if(startDate.getTime() > endDate.getTime()) {
          let saveDate = startDate
          startDate = endDate
          endDate = saveDate
        }
      }

      for (let key = 1; key <= lastDayCurrentMonth.getDate(); key++) {
        let dateCur = new Date(date.getFullYear(), date.getMonth(), key)

        if(checkDate) {
          if (isCurrentMonth)
            days.push({title: key, selected: (dateCur >= startDate && dateCur <= endDate), status: key < this.currentDate.getDate() ? 'past' : 'current'})
          else
            days.push({title: key, selected: (dateCur >= startDate && dateCur <= endDate), status: 'current'})
        } else {
          if (isCurrentMonth)
            days.push({title: key, selected: false, status: key < this.currentDate.getDate() ? 'past' : 'current'})
          else
            days.push({title: key, selected: false, status: 'current'})
        }
      }

      if (firstDay.getDay() !== 0) {
        lastMonth = firstDay.getMonth() !== 0 ?
            new Date(date.getFullYear(), firstDay.getMonth() - 1, 1) :
            new Date(date.getFullYear() - 1, 0, 1)
        let lastDayLastMonth = new Date(lastMonth.getFullYear(), lastMonth.getMonth() + 1, 0)
        for (let key = firstDay.getDay(); key !== 1; key--) {
          days.unshift({title: lastDayLastMonth.getDate() - (firstDay.getDay() - key), selected: false, status: 'old'})
        }
      }

      const months = ['Январь', 'Февраль', 'Март', 'Апрель', 'Май', 'Июнь', 'Июль', 'Август', 'Сентябрь', 'Октябрь', 'Ноябрь', 'Декабрь']
      let nameMonth = months[date.getMonth()]
      return {
        days,
        nameMonth,
        date
      }
    },
    select(id, calendar) {
      if (this.firstSelect && this.secondSelect) this.clear()
      if (this.multiplySelection) {
        this.clear()
        calendar.days[id].selected = !calendar.days[id].selected
        if (calendar.days[id].selected) {
          this.firstSelect = {
            calendar, id
          }
          this.$emit('update:modelValue', {
            firstDate: this.getSimpleDateFirst.getTime()
          })
        } else {
          this.firstSelect = null
          this.$emit('update:modelValue', null)
        }

      } else {
        if (!this.firstSelect) {
          calendar.days[id].selected = true
          this.firstSelect = {id, calendar}
          this.secondSelect = null
        } else {
          if (!this.secondSelect) {
            calendar.days[id].selected = true
            this.secondSelect = {id, calendar}
          } else {
            this.firstSelect.calendar.days[this.firstSelect.id].selected = false
            this.secondSelect.calendar.days[this.secondSelect.id].selected = false
            this.secondSelect = null
            calendar.days[id].selected = true
            this.firstSelect = {id, calendar}
          }
        }
      }

      if (this.firstSelect && this.secondSelect) {
        this.$emit('update:modelValue', {
          firstDate: this.getSimpleDateFirst.getTime(),
          secondDate: this.getSimpleDateSecond.getTime()
        })
        this.fill()
      }
    },
    fill(clear = true) {
      if (!this.firstSelect || !this.secondSelect) return
      let startDate = new Date(this.firstSelect.calendar.date.getFullYear(), this.firstSelect.calendar.date.getMonth(), this.firstSelect.calendar.days[this.firstSelect.id].title)
      let endDate = new Date(this.secondSelect.calendar.date.getFullYear(), this.secondSelect.calendar.date.getMonth(), this.secondSelect.calendar.days[this.secondSelect.id].title)

      if(startDate.getTime() > endDate.getTime()) {
        let saveDate = startDate
        startDate = endDate
        endDate = saveDate
      }
      this.firstSelect.calendar.days.forEach((item, id) => {
        let date = new Date(this.firstSelect.calendar.date.getFullYear(), this.firstSelect.calendar.date.getMonth(), item.title)
        if (date.getTime() >= startDate.getTime() && date.getTime() <= endDate.getTime() && item.status !== 'old') this.firstSelect.calendar.days[id].selected = clear
      })
      this.secondSelect.calendar.days.forEach((item, id) => {
        let date = new Date(this.secondSelect.calendar.date.getFullYear(), this.secondSelect.calendar.date.getMonth(), item.title)
        if (date.getTime() >= startDate.getTime() && date.getTime() <= endDate.getTime() && item.status !== 'old') this.secondSelect.calendar.days[id].selected = clear
      })
    },
    clear(){
      this.firstCalendar.days.forEach((item, id) => this.firstCalendar.days[id].selected = false)
      this.secondCalendar.days.forEach((item, id) => this.secondCalendar.days[id].selected = false)
      this.firstSelect = null
      this.secondSelect = null
    }
  },
  mounted() {
    this.$emit('input', this.selected);
    let date = new Date()
    let firstDay = new Date(date.getFullYear(), date.getMonth(), 1)
    this.firstCalendar = this.render(firstDay)
    let nextMonth = new Date(date.getFullYear(), date.getMonth() + 1, 1)
    this.secondCalendar = this.render(nextMonth)
  }
}
</script>

<style scoped>

</style>