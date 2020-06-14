<script>
  import BigHeader from "./components/BigHeader.svelte";
  import PhotoList from "./components/PhotoList.svelte";
  import data from "./instagram.json";
  export let hashtag;
</script>

<style>

</style>

<svelte:head>
  <link
    href="https://cdnjs.cloudflare.com/ajax/libs/bulma/0.8.0/css/bulma.min.css"
    rel="stylesheet" />
</svelte:head>

<main class="container">
  <BigHeader {hashtag} />
  <input type="text" bind:value={hashtag} />
  <PhotoList />
</main>
