<script>
  let color = "";
  let foods = [];
  function changeColor() {
    alert(color + "が選択されたときの処理");
  }
</script>

<p>color:{color}</p>
<select bind:value={color} on:change={changeColor}>
  <option value="" disabled>選択してください</option>
  <option value="red">赤</option>
  <option value="blue">青</option>
  <option value="green">緑</option>
</select>
<hr />
<p>food:{foods}</p>
<select multiple bind:value={foods}>
  <option value="" disabled>選択してください(複数可)</option>
  <option value="breakfast">朝食</option>
  <option value="lunch">昼食</option>
  <option value="dinner">夕食</option>
</select>
