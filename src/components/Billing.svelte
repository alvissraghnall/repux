<script>
import styles, { layout } from "../style";
import { assetsDir } from "../constants";
</script>

<section id="billing" class="{layout.sectionReverse}">
    <div class="{layout.sectionImgReverse}">
        <img src="{assetsDir + 'bill.png'}" alt="" class="w-full h-full relative z-[5]">

        <div class="absolute h-1/2 w-1/2 top-0 -left-1/2 z-[3] white__gradient rounded-full" />
        <div class="absolute h-1/2 w-1/2 bottom-0 -left-1/2 z-0 pink__gradient rounded-full" />

    </div>

    <div class="{layout.sectionInfo}">
        <h2 class="{styles.heading2}">Easily control your 
            <br class="hidden sm:block">
            billing and invoicing.
        </h2>
        <p class="mt-5 max-w-lg {styles.paragraph}">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Itaque aliquid accusantium sunt recusandae velit earum iusto dicta incidunt? Doloremque voluptatibus nobis nam dolorem aut possimus at velit. Est, nihil!
        </p>

        <div class="flex flex-row flex-wrap mt-6 sm:mt-10">
            <img src="{assetsDir + 'apple.svg'}" alt="apple store" class="h-11 w-32 object-contain mr-5 cursor-pointer">
            <img src="{assetsDir + 'google.svg'}" alt="play store" class="h-11 w-32 object-contain cursor-pointer">
        </div>
    </div>
</section>