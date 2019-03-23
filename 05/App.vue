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
  grid-template-columns: repeat(3, 1fr);
  grid-auto-rows: minmax(150px, auto);
  grid-gap: 10px;
  max-width: 960px;
  margin: 0 auto;
  /* align-items: stretch; */
  /* align-items: end; */
  /* justify-items: start; */
  /* justify-items: end; */
}

#content div {
  background: #3bbced;
  padding: 30px;
}

#content div:nth-child(even) {
  background: #777;
}

.one {
  align-self: end;
  justify-self: end;
}
.two {
  align-self: center;
  justify-self: center;
}
.three {
  align-self: start;
  justify-self: start;
}
</style>
