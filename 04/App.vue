<template lang='pug'>
  #app
    #content
      div 1
      div 2
      div 3 
      div.nested
        p 1
        p 2
        p 3
        p 4
      div 5
      div 6
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
  grid-template-columns: repeat(3, 1fr);
  
  grid-gap: 10px;
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
.nested {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 10px;
  /* grid-column: 1 / 4; */
  grid-column: span 3;
}
.nested p {
  border: 1px solid #fff;
  padding: 20px;
  margin: 0;
}
</style>
