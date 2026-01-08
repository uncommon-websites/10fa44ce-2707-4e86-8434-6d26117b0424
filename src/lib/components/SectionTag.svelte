<script lang="ts">
  export let text: string;
  export let color: string = "text-blue-600";
  export let icon: string | null = null;
</script>

<div class="flex items-center gap-2 mb-4">
  {#if icon}
    {@html icon}
  {/if}
  <span class="{color} font-bold text-xs tracking-widest uppercase">{text}</span>
</div>
