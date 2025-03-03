<template>
  <div class="container">
    <div class="text-display">
      {{ displayText }}
    </div>
    <button class="action-button" @click="handleClick">点击生成故事</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      displayText: '这里将显示生成的故事...'
    }
  },

  methods: {
    handleClick () {
      console.log('按钮被点击了')
    }
  }
}
</script>

<style scoped>
.container {
  padding: 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  min-height: 100vh;
  box-sizing: border-box;
}

.text-display {
  width: 90%;
  height: 60vh;
  margin: 20px auto;
  padding: 15px;
  border: 1px solid #ddd;
  border-radius: 8px;
  background-color: #f9f9f9;
  font-size: 16px;
  line-height: 1.6;
  overflow-y: auto;
}

.action-button {
  width: 80%;
  padding: 15px 0;
  background-color: #4CAF50;
  color: white;
  border: none;
  border-radius: 25px;
  font-size: 16px;
  margin-bottom: 30px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.2);
}

.action-button:active {
  opacity: 0.8;
}
</style>
