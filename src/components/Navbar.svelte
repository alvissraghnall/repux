<script>
import { navLinks, assetsDir } from "../constants";
$: toggle = false;
</script>

<style>
    
    
</style>

<nav class="w-full flex py-6 justify-between items-center">
    <img 
        src={assetsDir + "company-2.png"} 
        alt=""
        class="w-[180px] h-[80px] sm:h-[60px]"    
    >
    <ul class="list-none sm:flex hidden justify-end items-center flex-1">
        {#each navLinks as nL,i}
            <li 
                class="text-base text-white cursor-pointer font-poppins font-normal"
                class:mr-5="{i === navLinks.length - 1}"
                class:mr-10={i !== navLinks.length - 1}
            >
                <a href={`#${nL.id}`}>
                    {nL.title}
                </a>
                
            </li>
        {/each}
    </ul>

    <div class="flex flex-1 justify-end items-center sm:hidden">
        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <img 
            src={toggle ? assetsDir + "close.svg" : assetsDir + "menu.svg" } 
            alt=""
            class="object-contain h-7 w-7 mr-2 cursor-pointer"    
            on:click={() => toggle = !toggle}
        >
        <div class={`${toggle ? 'flex' : 'hidden'} p-6 bg-black-gradient absolute top-20 right-0 mx-4 my-2 min-w-[144px] rounded-xl sidebar`}>
            <ul class="list-none flex flex-col justify-end items-center flex-1">
                {#each navLinks as nL,i}
                    <li 
                        class="text-base text-white cursor-pointer font-poppins font-normal"
                        class:mr-0="{i === navLinks.length - 1}"
                        class:mb-4={i !== navLinks.length - 1}
                    >
                        <a href={`#${nL.id}`}>
                            {nL.title}
                        </a>
                        
                    </li>
                {/each}
            </ul>
        </div>

    </div>
</nav>