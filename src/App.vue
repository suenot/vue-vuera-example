<template>
  <div id="app">
    <h1></h1>
    <MyVueComponent msg="I'm a Vue component"/>
    <my-react-component />
    <!-- <my-react-component :message="message" @reset="reset" /> -->
  </div>
</template>

<script>
import MyVueComponent from './components/MyVueComponent.vue'
import MyReactComponent from './components/MyReactComponent'

export default {
  name: 'app',
  components: {
    MyVueComponent,
    'my-react-component': MyReactComponent
  }
}
</script>
