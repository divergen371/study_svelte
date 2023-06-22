<script>
  import { beforeUpdate, onMount, onDestroy, afterUpdate } from "svelte";
  beforeUpdate(() => {
    console.log("beforeUpdate");
  });
  onMount(() => {
    console.log("onMount");
  });
  afterUpdate(() => {
    console.log("afterUpdate");
  });
  onDestroy(() => {
    console.log("onDestroy");
  });
  console.log("Toplevel")

  let text = "テキスト";
  function updateText() {
    console.log("updateText関数実行");
    text = new Date().toLocaleString();
  }
</script>


<p>Text:{text}</p>
<button on:click={updateText}>更新</button>