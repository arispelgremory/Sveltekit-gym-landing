<script>
    import * as Icon from "lucide-svelte";
</script>

<div class="flex items-center justify-center gap-2 text-base">
    <p>4.6</p>
    { #each [0,1,2,3,4] as index }
        <div class="grid place-items-center-relative">
            <div class={
                    "grid place-items-center " + 
                    (index === 4 ? "w-3/5 overflow-hidden": " ")
                }>
                    <Icon.StarIcon color="#E6F285" />
                </div>
        </div>
    {/each}
    <p>500+</p>
</div>