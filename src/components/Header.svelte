<script>
  import { MenuIcon } from "lucide-svelte";

</script>

<header class="flex flex-col relative z-20">
    <div class="max-w-[1400px] max-auto w-full flex items-center justify-between p-4 py-6">
        <a href="/">
            <h1 class="font-semibold">
                Swoley <span class="text-indigo-400">Moley</span>
            </h1>
        </a>
        <button class="md:hidden grid items-center">
            <MenuIcon />    
        </button>
        <nav class="hidden md:flex items-center gap-4 lg:gap-6">
            <a class="duration-200 hover:text-indigo-400 cursor-pointer" href="#product">Product</a>
            <a class="duration-200 hover:text-indigo-400 cursor-pointer" href="#reviews">Reviews</a>
            <a class="duration-200 hover:text-indigo-400 cursor-pointer" href="#faqs">FAQs</a>
            <button class="call-to-action">
                Start free today
            </button>
        </nav>
    </div>
</header>