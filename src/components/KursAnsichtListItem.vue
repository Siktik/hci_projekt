<template>
  <div>

<li v-for="elem in testdata" v-bind:key="elem" id="listelement" @click="toggle">

<item class= "Kursname"> {{elem["Titel"]}} </item>
<item class= "KursStatus"> {{elem["Angemeldet"]}}</item>


</li>



</div>

</template>
<script>
export default {
name: 'KursAnsichtListItem',
data:()=>({
testdata:{Logik:{ Titel : "Logik", Angemeldet: "Angemeldet"}
  ,Mathe:{ Titel : "Mathe", Angemeldet: ""},
  Programmierung:{ Titel : "Programmierung", Angemeldet: "Angemeldet"}
},
  active:false

}),
methods:{
  toggle(){
    this.active = ! this.active
  }
}
}
</script>
<style>
#listelement {
  list-style-type: none;

  margin: 0;
  padding: 0;
}

#listelement {
  font: 200 20px/1.5 Helvetica, Verdana, sans-serif;
  border-bottom: 1px solid #ccc;
}

#listelement:last-child {
  border: none;
}

#listelement {
  text-decoration: none;
  color: #000;
  display: block;
  width: 200px;

  -webkit-transition: font-size 0.3s ease, background-color 0.3s ease;
  -moz-transition: font-size 0.3s ease, background-color 0.3s ease;
  -o-transition: font-size 0.3s ease, background-color 0.3s ease;
  -ms-transition: font-size 0.3s ease, background-color 0.3s ease;
  transition: font-size 0.3s ease, background-color 0.3s ease;
}

#listelement:hover {
  font-size: 30px;
  background: #f6f6f6;
}

</style>
