<template lang="html">
    <header class="main-header-section">
      <a href="#default" class="logo">CompanyLogo</a>

      <div class="main-header-right">
        <a href="#home">Home</a>
        <a href="#contact">Contact</a>
        <a href="#about">About</a>
      </div>

    </header>
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
  },
}
</script>