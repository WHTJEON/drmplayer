<template>
  <div class="stats">
    <table class="" style="width:100%">
      <tr>
        <td>Active Resolution</td>
        <td style="text-align:right;">{{resolution}}</td>
      </tr>
      <tr>
        <td>Bitrate</td>
        <td style="text-align:right;">{{stats.bitrate}}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: 'stats',
  props: ['stats', 'buffer'],
  data() {
    return {
    };
  },
  computed: {
    resolution() {
      return `${this.stats.width || 0} x ${this.stats.height || 0}`;
    },
  },
  methods: {
  },
};
</script>

<style scoped>
</style>
