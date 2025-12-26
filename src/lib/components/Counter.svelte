<script lang="ts">
  let value = $state(0);
</script>

<button type="button" class="border px-2 py-1 cursor-pointer rounded-md" onclick={() => value++}>
  Click me: {value}
</button>
