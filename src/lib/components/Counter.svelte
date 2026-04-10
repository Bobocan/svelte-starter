<script lang="ts">
  let {
    value = $bindable(0),
  }: {
    value?: number;
  } = $props();
</script>

<button type="button" class="border px-2 py-1 cursor-pointer rounded-md" onclick={() => value++}>
  Click me: {value}
</button>
