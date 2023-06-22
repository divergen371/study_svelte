<script>
  const messages = [
    { id: 1, message: "message1" },
    { id: 2, message: "message2" },
    { id: 3, message: "message3" },
  ];
</script>

{#each messages as message}
  <p>{message.id}:{message.message}</p>
{/each}
