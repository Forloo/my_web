<script>
  let name = "";
  let count = 0;

  const incrementCounter = () => {
    count += 1;
  };
  const handleInput = (event) => {
    name = event.target.value;
  };
  const resetName = () => {
    name = "Unkown";
  };
</script>

<main>
  <h1>Hello {name}</h1>
  <input type="text" on:input={handleInput} />
  <button on:click={resetName}>Set name to Unknown</button>
</main>

<style>
  main {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>
