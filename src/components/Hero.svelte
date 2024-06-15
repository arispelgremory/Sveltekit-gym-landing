<script>
  import SectionWrapper from "./SectionWrapper.svelte";
  import Header from "./Header.svelte";
  import Cta from "./CTA.svelte";
  import * as Icon from "lucide-svelte";
</script>


<SectionWrapper>
    <Header />
    <div class="flex flex-col gap-10 flex-1 items-center justify-center pb-10 md:pb-14">
        <h2 class="text-5xl sm:text-6xl md:text-7xl lg:text-8xl mx-auto text-center w-full max-w-[1200px] font-semibold">
            <span class="text-indigo-400">
                Gym
            </span>
            Training
            <span class="text-slate-600 line-through">Is Hard</span>
            <br>
            Just Got
            <span class="text-indigo-400">
                Easier
            </span>
        </h2>
        <p class="text-xl sm:text-2xl md:text-3xl text-center mx-auto w-full max-w-[1000px]">
            Less thinking & more doing. We're the trainer in your pocket full of 
            <span class="italic">personalized workouts, exercise explainations, analytics</span>
            and much much more.
        </p>
        <Cta />
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
    </div>
</SectionWrapper>