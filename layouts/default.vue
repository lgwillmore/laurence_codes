<template>
  <b-container-fluid>
    <div sticky-container>
      <b-row>
        <b-col cols="12">
          <page-header/>
        </b-col>
      </b-row>
      <b-row class="m-2">
        <b-col md="10" offset-md="1">
          <nuxt/>
        </b-col>
      </b-row>
    </div>
  </b-container-fluid>
</template>

<script lang="ts">
    import {Component, Vue} from "vue-property-decorator"
    import PageHeader from "~/layouts/partials/PageHeader.vue"

    @Component({
        components: {PageHeader},
    })
    export default class Default extends Vue {

    }
</script>

<style>
  html {
    font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }

  *,
  *:before,
  *:after {
    box-sizing: border-box;
    margin: 0;
  }

  .button--green {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #3b8070;
    color: #3b8070;
    text-decoration: none;
    padding: 10px 30px;
  }

  .button--green:hover {
    color: #fff;
    background-color: #3b8070;
  }

  .button--grey {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #35495e;
    color: #35495e;
    text-decoration: none;
    padding: 10px 30px;
    margin-left: 15px;
  }

  .button--grey:hover {
    color: #fff;
    background-color: #35495e;
  }
</style>
