<script lang="ts">
  export let handleClick: () => void;
</script>

<button on:click={handleClick}>
  <slot />
</button>

<style>
  button {
    background-color: red;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  button:hover {
    background-color: rgb(207, 2, 2);
  }
  button:active {
    background-color: rgb(255, 93, 93);
  }
</style>
