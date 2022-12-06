<script>
    import { features } from "../constants/index";
    import Button from "../shared/Button.svelte";
    import FeatureCard from "../shared/FeatureCard.svelte";
    import styles, { layout } from "../style";
</script>

<section id="features" class={layout.section}>
    <div class="{layout.sectionInfo}">
        <h2 class={styles.heading2}>
            You do the business, ,<br class="hidden sm:block"> we'll handle the money.
        </h2>
        <p class="{styles.paragraph} max-w-lg mt-5">
            With the rright Credit Card, you can improve your financial life by building credit, earning rewards and saving money. But with Hundreds of Credit Cards on the market.
        </p>

        <Button class="mt-10" />
    </div>

    <div class="flex-col {layout.sectionImg}">
         {#each features as feature,index}
            <FeatureCard 
                {feature} 
                {index} 
                featuresLength={features.length} 
                {styles}
            />
         {/each}
    </div>
</section>