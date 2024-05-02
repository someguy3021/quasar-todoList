<template>
  <q-page class="bg-grey-3 colunm">
    <q-list>

      <q-item
      v-for="task in tasks" :key="task.title"
      tag="label" v-ripple>
        <q-item-section avatar>
          <q-checkbox v-model="color" val="teal" color="primary" />
        </q-item-section>
        <q-item-section>
          <q-item-label>{{task.title}}</q-item-label>
          <q-item-label caption>With description</q-item-label>
        </q-item-section>
      </q-item>

    </q-list>
  </q-page>
</template>

<script>
export default{
  data() {
    return{
      tasks:[
        {
          title: 'Hello1',
          done: false,
        },
        {
          title: 'Hello2',

          done: false,
        }
      ]
    };
  },
};
</script>
