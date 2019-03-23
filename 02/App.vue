<template lang='pug'>
  #app
    #content
      div 1
      div 2
      div Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
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
  /* grid-auto-rows: 200px; */
  /* grid-auto-rows: minmax(200px, auto); */
  /* grid-template-rows: 200px 300px 400px 200px; */
  /* grid-template-rows: repeat(3, 200px); */
  grid-template-rows: repeat(3, minmax(200px, auto));
  /* grid-column-gap: 10px;
  grid-row-gap: 10px; */
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
</style>
