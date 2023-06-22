<script>
  let isAgree = false;
  let vegetables = [];
  let size = "medium";
</script>

<input type="checkbox" name="" id="" bind:checked={isAgree} />利用規約に同意する
<input type="button" value="次へ" disabled={!isAgree} />
<hr />
<p>vegetables:{vegetables}</p>
<input type="checkbox" value="tomato" bind:group={vegetables} />tomato
<input type="checkbox" value="carrot" bind:group={vegetables} />carrot
<input type="checkbox" value="onion" bind:group={vegetables} />onion
<hr />
<p>size:{size}</p>
<input type="radio" value="large" bind:group={size}>large
<input type="radio" value="medium" bind:group={size}>medium
<input type="radio" value="small" bind:group={size}>small
