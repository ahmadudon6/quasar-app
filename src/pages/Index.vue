<template>
  <q-page class="row items-center justify-evenly">
    <example-component
      title="Welcome to quasar"
      active
      :todos="todos"
      :meta="meta"
    ></example-component>
  </q-page>
</template>

<script lang="ts">
import ExampleComponent from 'components/CompositionComponent.vue'
import { Todo, Meta } from 'components/models'

export default {
  name: 'PageIndex',
  components: { ExampleComponent },
  data () {
    const todos: Todo[] = [
      {
        id: 1,
        content: 'ct1'
      },
      {
        id: 2,
        content: 'ct2'
      },
      {
        id: 3,
        content: 'ct3'
      },
      {
        id: 4,
        content: 'ct4'
      },
      {
        id: 5,
        content: 'ct5'
      }
    ]
    const meta: Meta = {
      totalCount: 1200
    }
    return { todos, meta }
  }
}
</script>
