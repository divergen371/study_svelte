<script>
  let items = [
    { id: 0, name: "要素1" },
    { id: 1, name: "要素2" },
    { id: 2, name: "要素3" },
  ];

  function deleteItem() {
    const newItems = [...items];
    newItems.splice(0, 1);
    items = newItems;
  }
</script>

{#each items as item (item.id)}
  <p><input type="checkbox" />{item.name}</p>
{/each}

<button on:click={deleteItem}>削除</button>
