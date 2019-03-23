<template lang='pug'>
  #app
    #content
      div.one 1
      div.two 2
      div.three 3 
      div.four 4
      div.five 5
      div.six 6
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
  grid-template-columns: repeat(6, 1fr);
  grid-template-rows: repeat(4, minmax(150px, auto));
  
  grid-gap: 10px;
  max-width: 960px;
  margin: 0 auto;
}

#content div {
  background: #3bbced;
  padding: 30px;
  /* margin: 20px; */
}

#content div:nth-child(even) {
  background: #777;
}
.one {
  /* grid-column-start: 1;
  grid-column-end: 3; */
  grid-column: 1 / 3;
}
.two {
  grid-column: 3 / 7;
}
.three {
  grid-column: 1 / 4;
  grid-row: 2 / 4;
}
.four {
  grid-column: 4 / 7;
  grid-row: 2 / 4;
}
.five {
  grid-column: 3 / 7;
  grid-row: 4 / 6;
}
.six {
  grid-column: 1 / 3;
  grid-row: 4 / 6;
}
</style>
