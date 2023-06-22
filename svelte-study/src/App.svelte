<script>
  // あえて値の型と変数名の関連性をあべこべにする
  let text = 10;
  let number = "10";
  function checkType() {
    console.log(text, typeof text);
    console.log(number, typeof number);
  }
</script>

<p>text:<input type="text" bind:value={text} /></p>
<p>number:<input type="number" bind:value={number} /></p>
<button on:click={checkType}>型チェック</button>
