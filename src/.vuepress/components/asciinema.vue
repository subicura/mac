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
      loadCount: 0
    };
  },
  mounted() {
    if (!window.asciinema) {
      var css = document.createElement("link");
      css.href = "/css/asciinema-player.css";
      css.rel = "stylesheet";
      document.body.appendChild(css);

      var js = document.createElement("script");
      js.src = "/js/asciinema-player.2.6.1.js";
      document.body.appendChild(js);
    }
    this.load();
  },
  destroyed() {
    const current = document.getElementById(this.id);
    if (window.asciinema && window.asciinema.player && window.asciinema.player.js && current) {
        window.asciinema.player.js.UnmountPlayer(current);
      }
  },
  methods: {
    load() {
      if (window.asciinema && window.asciinema.player && window.asciinema.player.js) {
        const current = document.getElementById(this.id);
        window.asciinema.player.js.CreatePlayer(current, this.src, {
          autoPlay: false,
          loop: false,
          title: this.title,
        });
      } else {
        setTimeout(() => {
          if (this.loadCount < 5) {
            this.load();
            this.loadCount++;
          }
        }, this.loadCount * 100 + 50);
      }
    },
  },
};
</script>
