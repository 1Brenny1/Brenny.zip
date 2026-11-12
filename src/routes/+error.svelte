<script lang="ts">
    import { page } from "$app/state";
    import { House } from "@lucide/svelte";
</script>

<div class="w-full flex flex-col justify-center items-center gap-8 h-1/2">
    <h2 class="text-9xl">{page.status}</h2>
    <hr class="hr w-md">
    <p class="text-2xl">{page.error?.message}</p>

    <a href="/" class="btn preset-tonal-brand flex gap-2 p-4 w-1/3">
        <House />
        Go Home
    </a>
</div>