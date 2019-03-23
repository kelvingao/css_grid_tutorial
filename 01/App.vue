<template lang='pug'>
  #app
    #content
      div 1
      div 2
      div 3
      div 4
      div 5
      div 6
      div 7
      div 8
      div 9
</template>

<script>

export default {
  name: 'app',
 
}
</script>

<style>
body {
  color: #fff;
  font-family: 'Nunito Semibold';
  text-align: center;
}

#content {
  display: grid;
  /* grid-template-columns: 30% 20% 50%; */
  /* grid-template-columns: 1fr 2fr 1fr; */
  grid-template-columns: repeat(3, 1fr);
  max-width: 960px;
  margin: 0 auto;
}

#content div {
  background: #3bbced;
  padding: 30px;
}

#content div:nth-child(even) {
  background: #777;
}
</style>
