<template lang="html">
    <footer class="main-footer-section">
        <ol v-if="canSee">
            <li v-for="x in objArr" :key="x.id"> {{x.val}}</li>
        </ol>
    </footer>
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
    }
  }
}
</script>