<template>
  <div class="terminal mx-auto">
    <div id="terminal-body">
      <div id="terminal-player-wrapper"></div>
    </div>
    <div id="terminal-buttons">
      <div class="flex flex-wrap justify-center">
        <button
          v-for="cast in casts"
          :key="cast.src"
          class="bg-primary-color-500 text-white font-semibold m-1 p-1 rounded"
          style="width: 100px"
          @click="handleClick(cast.src, cast.cols, cast.rows)"
        >
          <span class="mr-1">{{ cast.title }}</span>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Terminal',

  data() {
    return {
      casts: [
        { title: 'Cluster', src: '/cluster-create.cast', cols: 109, rows: 29 },
        { title: 'Services', src: '/osctl-services.cast', cols: 109, rows: 29 },
        { title: 'Routes', src: '/osctl-routes.cast', cols: 109, rows: 29 },
        {
          title: 'Interfaces',
          src: '/osctl-interfaces.cast',
          cols: 109,
          rows: 29
        },
        {
          title: 'Containers',
          src: '/osctl-containers.cast',
          cols: 109,
          rows: 29
        },
        {
          title: 'Processes',
          src: '/osctl-processes.cast',
          cols: 109,
          rows: 29
        },
        { title: 'Mounts', src: '/osctl-mounts.cast', cols: 109, rows: 29 }
      ]
    }
  },

  mounted() {
    const cast = this.casts[0]
    this.handleClick(cast.src, cast.cols, cast.rows)
  },

  methods: {
    handleClick(src, cols, rows) {
      const terminalPlayerWrapper = document.getElementById(
        'terminal-player-wrapper'
      )
      terminalPlayerWrapper.innerHTML =
        '<asciinema-player id="terminal-player" cols="' +
        cols +
        '"rows="' +
        rows +
        '" preload autoplay loop speed="1.0" font-size="small" src="' +
        src +
        '"></asciinema-player>'
    }
  }
}
</script>

<style>
#terminal-body {
  height: auto;
  width: auto;
}

.control-bar {
  display: none;
}
</style>
