<template>
  <footer>
    This resume source code is available at
    <a target="noopener" href="https://github.com/sixpounder/resume">
      https://github.com/sixpounder/resume
    </a>
  </footer>
</template>

<style lang="stylus" scoped>
footer
  @apply: block w-full text-center text-sm

  a
    @apply: text-indigo-600

    &:hover
      @apply: underline

    @media print
      color initial
      &:hover
          text-decoration none
</style>
