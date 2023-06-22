<script>
  const messages = [
    { id: 0, message: "message1" },
    { id: 1, message: "message2" },
    { id: 2, message: "message3" },
  ];
</script>

{#each messages as message ,i (message.id)}
  <p>[No {i + 1}]{message.message}</p>
{/each}
