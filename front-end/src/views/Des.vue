<template>
<div class="wrapper">
  <div class="States">
    <div class="state" v-for="state in States" :key="state.id">
      <div class="info">
        <h1>{{state.name}}</h1>
      </div>
      <div class="des">
        <h4>{{state.description}}</h4>
      </div>
    </div>
  </div>
</div>
</template>


<script>
export default {
  name: 'Des',
  props: {
    States: Array
  }
}
</script>

<style scoped>
.wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
}

.States {
  margin-top: 20px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.state {
  margin: 10px;
  margin-top: 50px;
  width: 200px;
}


.info {
  background: red;
  color: #000;
  padding: 10px 30px;
  height: 40px;
}

.info h1 {
  font-size: 16px;
}

.info h2 {
  font-size: 14px;
}

.info p {
  margin: 0px;
  font-size: 10px;
}

button {
  height: 50px;
  background: #000;
  color: white;
  border: none;
}

.auto {
  margin-left: auto;
}
</style>