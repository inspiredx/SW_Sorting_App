<template>
    <div id="app">

        <app-header/>

        <div class="container">
            <h1 class="pt-3 pb-3">Персонажи Star Wars</h1>

            <app-modal/>

            <spinner/>

            <div class="card mb-3" style="max-width: 540px;">
    <div class="row g-0">
      <div class="col-md-4">
        <img src="https://sun9-21.userapi.com/impg/y9IsEXM7CqJkYY4LX_Ydui3Yrimi1cEf8p_5qQ/7A1vzs-jBoc.jpg?size=368x416&quality=96&sign=9629c7bfef9ca9094f5b789dd0fffd12&type=album" class="img-fluid rounded-start" alt="Аген Колар">
      </div>
      <div class="col-md-8">
        <div class="card-body">
          <h5 class="card-title">Аген Колар</h5>
          <!-- Button trigger modal -->
          <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
            Подробней
          </button>
        </div>
      </div>
    </div>
  </div>
        </div>

    </div>
</template>

<script>
    import Spinner from "./components/Spinner";
    import AppModal from "./components/AppModal";
    import AppHeader from "./components/AppHeader";

    export default {
        name: 'App',
        components: {
            AppHeader,
            AppModal,
            Spinner,
        },
        data() {
            return {
                loading: false,
                characters: [],
                characterIndex: 0,
            }
        },
        methods: {},
        computed: {},
    }
</script>

<style>

</style>
