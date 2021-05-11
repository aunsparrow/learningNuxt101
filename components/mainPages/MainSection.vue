<template lang="html">
    <section class="main-section-section">
        <ol v-if="canSee">
            <li v-for="x in objArr" :key="x.id"> {{x.val}}</li>
        </ol>
        <b-button variant="success" @click="clickConsole">{{msg2}}</b-button>
    </section>
</template>

<script>
export default {
    data() {
    return {
      message: 'test message',
      canSee: true,
      objArr: [
        { id: 1, val: 'test1', fax: true },
        { id: 2, val: 'test2', fax: false },
        { id: 3, val: 'test3', fax: true },
      ],
      msg1:'Text',
      msg2: String(process.env.BASE_URL)
    }
  },
  methods:{
    clickConsole(){
      console.log("process",process.env.BASE_URL)
      console.log("env",process.env.NODE_ENV)
    }

  },
  computed:{
    nodeEnv(){
      return this.msg1 = process.env.NODE_ENV
    }
  }
}
</script>