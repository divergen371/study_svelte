<script>
  let message = undefined;
</script>

{#if message}
  <p>message:{message}</p>
{:else}
  <p>messgeにFalsyな値が代入されています</p>
{/if}
