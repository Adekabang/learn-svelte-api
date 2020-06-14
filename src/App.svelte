<script>
  import BigHeader from "./components/BigHeader.svelte";
  import PhotoList from "./components/PhotoList.svelte";
  import data from "./instagram.json";
  export let hashtag;
</script>

<style>

</style>

<main>
  <BigHeader {hashtag} />
  <input type="text" bind:value={hashtag} />
  <PhotoList />
</main>
