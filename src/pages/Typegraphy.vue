<template>
  <q-page class="flex column q-pa-md">
    <!-- <h3>Typegraphy</h3> -->
    <span class="text-h1">Typegraphy 1</span>
    <span class="text-h2">Typegraphy 2</span>
    <span class="text-h3">Typegraphy 3</span>
    <span class="text-h4">Typegraphy 4</span>
    <span class="text-h5">Typegraphy 5</span>
    <span class="text-h6">Typegraphy 6</span>

    <q-separator/>

    <span class="text-weight-thin"> Lorem ipsum dolor sit amet consectetur, adipisicing elit. Esse, sequi a libero rem eligendi consectetur laborum aliquam inventore quibusdam magni sint quod deleniti debitis voluptate modi minima at ipsa animi!</span>
    <span class="text-weight-light"> Lorem ipsum dolor sit amet consectetur, adipisicing elit. Esse, sequi a libero rem eligendi consectetur laborum aliquam inventore quibusdam magni sint quod deleniti debitis voluptate modi minima at ipsa animi!</span>
    <span class="text-weight-regular"> Lorem ipsum dolor sit amet consectetur, adipisicing elit. Esse, sequi a libero rem eligendi consectetur laborum aliquam inventore quibusdam magni sint quod deleniti debitis voluptate modi minima at ipsa animi!</span>
    <span class="text-weight-medium"> Lorem ipsum dolor sit amet consectetur, adipisicing elit. Esse, sequi a libero rem eligendi consectetur laborum aliquam inventore quibusdam magni sint quod deleniti debitis voluptate modi minima at ipsa animi!</span>
    <span class="text-weight-bold"> Lorem ipsum dolor sit amet consectetur, adipisicing elit. Esse, sequi a libero rem eligendi consectetur laborum aliquam inventore quibusdam magni sint quod deleniti debitis voluptate modi minima at ipsa animi!</span>
    <span class="text-weight-bolder"> Lorem ipsum dolor sit amet consectetur, adipisicing elit. Esse, sequi a libero rem eligendi consectetur laborum aliquam inventore quibusdam magni sint quod deleniti debitis voluptate modi minima at ipsa animi!</span>


    <q-btn color="primary" label="Abrir menú" class="q-mt-md" @click="toggleSideMenu" />
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';

import useUI from '../composables/useUI'

export default defineComponent({
  name: 'Typegraphy',

  setup () {
    //const leftDrawerOpen = ref(false)
    const {sideMenuOpen, toggleSideMenu} = useUI()


    return {
      sideMenuOpen, 
      toggleSideMenu
    }
  }
})
</script>
