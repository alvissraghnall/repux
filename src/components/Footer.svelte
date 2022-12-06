<script>
import styles, { layout } from "../style";
import { assetsDir, footerLinks, socialMedia } from "../constants";
import Button from "../shared/Button.svelte";
</script>

<section class=" flex-col {styles.flexCenter} {styles.paddingY}">
    <div class="mb-8 w-full md:flex-row {styles.flexStart}">
        <div class="flex flex-1 flex-col justify-start mr-10">
            <img 
                src={assetsDir + "company-2.png"} 
                alt=""
                class="w-64 h-[9rem] object-contain"    
            >
            <p class="font-poppins font-normal {styles.paragraph} mt-4 max-w-xs">
                A new way to make payments fast, secure && easy!
            </p>
        </div>

        <div class="w-full flex-row flex justify-between flex-wrap mt-10 md:mt-0 flex-[1.5]">
            {#each footerLinks as link}
                <div class="flex flex-col ss:my-0 my-4 min-w-[150px]">
                    <h4 class="text-lg font-poppins font-medium text-white">
                        {link.title}
                    </h4>
                    <ul class="list-none mt-4">
                        {#each link.links as linkItem,i}
                            <li class="text-base font-poppins font-normal text-dimWhite hover:text-secondary cursor-pointer {i !== link.links.length -1 ? 'mb-4' : 'mb-0'}">
                                {linkItem.name}
                            </li>
                        {/each}
                    </ul>
                </div>
            {/each}
        </div>
    </div>

    <div class="pt-6 w-full md:flex-row flex flex-col items-center border-t-2 justify-between border-t-[#3f3e45] ">
        <p class="text-base capitalize font-poppins font-normal text-white text-center">
            &copy; 2022 repux. all rights reserved.
        </p>

        <div class="flex mt-6 md:mt-0 flex-row">
            {#each socialMedia as icon,i}
                <img src="{icon.icon}" alt="{icon.id}" class="w-5 h-5 object-contain cursor-pointer {i !== socialMedia.length -1 ? 'mr-6' : 'mr-0'}">
            {/each}
        </div>
    </div>
</section>