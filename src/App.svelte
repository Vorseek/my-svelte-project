<script lang="ts">
  export let name: string;
  let value = 0;
</script>

<main>
  <h1>Hello {name}!</h1>
  <p>
    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
    how to build Svelte apps.
  </p>
  <button on:click={() => (value += 1)} class="btn btn-primary">Test {value}</button>
 
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }
  .btn {
    background-color: red;
    border-radius: 50%;
    width: 50px;
    height: 50px;
  }
  .btn:hover {
    background-color: blue;
  }
  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
