<script>
    export let card;
    import { assetsDir } from "../constants";
</script>

<div class="flex justify-between px-10 py-12 mr-0 my-5 sm:mr-5 flex-col md:mr-10 rounded-2xl max-w-sm">
    <img src="{assetsDir + 'quotes.svg'}" alt="" class="object-contain w-11 h-7">
    <p class="font-poppins font-normal text-white my-10 text-xl">
        {card.content}
    </p>

    <div class="flex-row flex">
        <img src="{card.img}" alt="" class="w-12 h-12 rounded-full">
        <div class="flex-col flex ml-4">
            <h4 class="font-poppins font-semibold text-white text-base">
                {card.name}
            </h4>
            <p class="font-poppins font-normal text-dimWhite text-base">
                {card.title}
            </p>
        </div>
    </div>

</div>