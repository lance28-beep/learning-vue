<script>
export default {
  name:"App",
  data(){
    return{
      count:0,
      greet:"Hello",
      channel: "Lance Coding",
      hack:`<a href="#" onclick="alert('You have been hacked!')">Win a prize!</a>`,
      headingId:'heading',
      isDisabled: false,
      status:'danger',
      isPromoted:true,
      isSoldout:false,
      highLightColor:'orange',
      headerSize:50,
      headerStyleObject:{
        color:'orange',
        fontSize:'50px',
        padding:'20px'
      }
    }
  }
}
</script>

<template>
  <button @click="count++">Count is: {{count}} : {{greet}}</button>
  <div v-html="hack"></div>
  <div v-bind:id="headingId">Heading</div>
  <div id="hello">lance</div>
  <button v-bind:disabled="isDisabled">{{isDisabled}}</button>
  <h2 class="underline">Underline Text</h2>
  <h2 class="underline" v-bind:class="status">Status</h2>
  <h2 v-bind:class="isPromoted && 'promoted'">Movie Promoted</h2>
  <h1 v-bind:class="isSoldout? 'sold-out':'new'">is soldOut?</h1>
  <h2 v-bind:class="['newStyle','new']">Newly promoted movie</h2>
  <h2 v-bind:class="{
    promoted:isPromoted,
    new:!isSoldout,
    'sold-out':isSoldout
  }">Object conditional movie</h2>

<h2 v-bind:style="{
  color:highLightColor,
  'font-size':headerSize + 'px',
  padding:'20px'
}">Inline Style</h2>

<h2 v-bind:style="headerStyleObject">heading Tag</h2>
</template>


<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}

.underline{
  text-decoration: underline;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}

.promoted{
  font-style: italic;
}

.sold-out{
  color: yellow;
  background: rgb(255, 0, 0);
}

.new{
  color: red;
  background: yellow;
}

.newStyle{
  font-style: italic;
  text-decoration: underline;
}
</style>
