<template>
  <div id="app">
    <a id="github" href="https://github.com/jkhaoqi110/yinyangshi-assistant" target="_blank"><img src="./assets/github.png"></a>
    <img src="./assets/logo.png">
    <router-view></router-view>
    <FooterComponent></FooterComponent>
  </div>
</template>

<script>
import FooterComponent from './components/Footer'

export default {
    name: 'app',
    components: {
        FooterComponent
    }
}
</script>

<style>
#app {
  font-family: 'Microsoft Yahei', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#github {
    position: absolute;
    top: 0.5rem;
    right: 0.5rem;

}
#github img{
    display: block;
    width: 1.8rem;
    height: 1.8rem;
    transition: opacity .3s ease;
    opacity: .7
}
#github img:hover{
    opacity: 1
}
.text-center input {
    text-align: center!important;
}
.text-center .mu-text-field-hint {
    left: 50%;
    margin-left: -25%;
}

</style>
