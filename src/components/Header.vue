<template>

<header id="head">
<h1> Testing </h1>
<nav id="nav">
  <ul id="test">
    <li>Test</li>
  </ul>
</nav>
</header>


</template>
<script>

export default {
name: 'Header',
components:{
},

}
</script>
<style>
#head {
    background-color: lightblue;
    text-align: center;
}
#nav{
  align-self: flex-end;
  font-size: 150%
}
#h1{
  position: absolute;
  align-content: center;
}
</style>
