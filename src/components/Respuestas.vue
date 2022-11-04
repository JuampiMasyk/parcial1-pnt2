<template>

  <section class="src-componentes-http-client">
    <div class="jumbotron">
      <h2>Componente HttpClient</h2>
      <hr>
      <hr>
      <br>
        <table class="table table-dark">
          <tr>
            <th>Numero</th>
            <th>Respuesta</th>
          </tr>
          <tr v-for="pregunta in preguntas" :key="pregunta[numero]">
            <td>{{ pregunta.numero }}</td>
            <td>{{ pregunta.respuestas }}</td>
          </tr>
        </table>

    </div>
  </section>

</template>

<script>

  export default  {
    name: 'src-componentes-respuestas',
    props: [],
    mounted () {

    },
    data () {
      return {
        preguntas : [
        { numero: 1, respuestas: ["b","d"] },
        { numero: 2, respuestas: ["c"] },
        { numero: 3, respuestas: ["b"] },
        ]
      }
    },
    methods: {

    },
    computed: {

    }
}


</script>

<style scoped lang="css">
  .src-componentes-respuestas {

  }

  .jumbotron {
    background-color: green;
    color: white;
  }
</style>