<script lang="ts">
  import Counter from "$lib/components/Counter.svelte";

  let value = $state(0);

  let valueSync = $state(0);
</script>

<h1>Welcome to SvelteKit</h1>

<div class="grid gap-4">
  <div class="flex gap-4">
    <Counter></Counter>
  </div>

  <div class="flex gap-4">
    <Counter bind:value></Counter>
    <div>The counter value is {value}</div>
  </div>

  <div class="flex gap-4">
    <Counter bind:value={valueSync}></Counter>
    <Counter bind:value={valueSync}></Counter>
  </div>
</div>

<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
