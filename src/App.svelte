<script>
  import BigHeader from "./components/BigHeader.svelte";
  import PhotoList from "./components/PhotoList.svelte";
  import data from "./instagram.json";
  export let hashtag;
</script>

<style>
  h1{
    color: #57A71c;
  }
</style>

<main>
  <BigHeader {hashtag} />
  <input type="text" bind:value={hashtag} />
	<h1>Photos</h1>
  <PhotoList />
</main>
