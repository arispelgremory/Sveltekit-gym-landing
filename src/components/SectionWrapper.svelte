<script>
    export let id; // Export prop
</script>

<section class={"min-h-screen flex flex-col px-4"}>
    <div class="flex flex-col flex-1 max-auto w-full max-w-[1400px]">
        <slot />
    </div>
</section>