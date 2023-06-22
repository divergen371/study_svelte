<script>
  const messages = [];
</script>

{#each messages as message}
  <p>{message.id}:{message.message}</p>
{:else}
  <p>メッセージはありません</p>
{/each}
