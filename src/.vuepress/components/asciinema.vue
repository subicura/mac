<template>
  <div class="asciinema-component">
    <div class="asciinema-terminal_wrapper">
      <div class="asciinema-terminal_header">
        <div style="flex: none; width: 65px; text-align: left">
          <span
            class="asciinema-terminal_btn asciinema-terminal_btn_1"
          ></span>
          <span
            class="asciinema-terminal_btn asciinema-terminal_btn_2"
          ></span>
          <span
            class="asciinema-terminal_btn asciinema-terminal_btn_3"
          ></span>
        </div>
        <div class="asciinema-terminal_title">{{ windowTitle }}</div>
        <div style="flex: none; width: 65px;" />
      </div>
      <div :id="id"></div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["id", "src", "title", "rows"],
  data() {
    return {
      windowTitle: this.title || "terminal",
    };
  },
  mounted() {
    const current = document.getElementById(this.id);
    if (window.asciinema && window.asciinema.player && window.asciinema.player.js) {
      window.asciinema.player.js.CreatePlayer(current, this.src, {
        autoPlay: false,
        loop: false,
        title: this.title,
      });
    }
  },
  destroyed() {
    const current = document.getElementById(this.id);
    if (window.asciinema && window.asciinema.player && window.asciinema.player.js && current) {
        window.asciinema.player.js.UnmountPlayer(current);
      }
  }
};
</script>
