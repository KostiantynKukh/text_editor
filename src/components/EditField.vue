<template>
  <div class="wrapper" >
    <div class="wrapper__text-content text-content" contenteditable='true'>
      <span v-for="word in wordContainer"
        class="text-content__text"
        :style="{
          fontSize: word.fontSize,
          color: word.color,
          background: word.backgrond
        }"       
        :key='word.id'        
      >
        {{ word.text }}
      </span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      wordContainer: [
        {
          id: 0,
          text: 'Hello',
          color: 'red',
          fontSize: '20px',
          backgrond: 'blue'
        },
        {
          id: 1,
          text: 'you',
          color: 'yellow',
          fontSize: '14px',
          backgrond: 'green'
        },
        {
          id: 2,
          text: 'can',
          color: 'blue',
          fontSize: '14px',
          backgrond: 'yellow'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.wrapper {
  max-width: 600px;
  margin: 50px auto;
  font-size: 20px;
}

.text-content {
  &__text {
    padding: 2px 10px;
    border-radius: 5px;
  }
}

</style>