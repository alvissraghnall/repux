<script>
    import styles, { layout } from "../style";
    import { assetsDir } from "../constants";
    import Button from "../shared/Button.svelte";
    import { feedback } from "../constants";
    import FeedbackCard from "../shared/FeedbackCard.svelte";
</script>

<section class="flex-col relative {styles.paddingY} {styles.flexCenter}">
    <div class="absolute z-0 blue__gradient w-3/5 rounded-full h-3/5 -right-1/2" />

    <div class="items-center md:flex-row sm:mb-16 w-full z-[1] relative mb-6 flex-col justify-between flex">
        <h1 class="{styles.heading2}">
            What people are <br class="sm:block hidden">
            saying about us.
        </h1>
        <div class="w-full mt-6 md:mt-0">
            <p class="{styles.paragraph} text-left max-w-md">
                Everything you need to accept payments & grow your business anywhere on the planet.
            </p>
        </div>
    </div>

    <div class="flex sm:justify-start flex-wrap justify-center w-full feedback-container relative z-[1]">
        {#each feedback as item,i (item.id)}
            <FeedbackCard card={item}  />
        {/each}
    </div>
</section>