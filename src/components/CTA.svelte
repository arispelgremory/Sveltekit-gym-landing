<script>
    export let dark;
</script>

<div class="flex items-center gap-4">
    <button class={"special-btn " + (dark ? " bg-[#181b34]" : " ")}>
        <p class="text-base sm:text-lg md:text-xl">Contact Us</p>
    </button>
    <button class="special-btn-dark">
        <p class="text-base sm:text-lg md:text-xl">Get Started &rarr;</p>
    </button>
</div>