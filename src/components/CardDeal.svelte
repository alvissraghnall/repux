<script>
    import styles, { layout } from "../style";
    import { assetsDir } from "../constants";
    import Button from "../shared/Button.svelte";
    
</script>

<section class="{layout.section}">
    <div class="{layout.sectionInfo}">
        <h2 class="{styles.heading2}">
            Find a better card deal <br class="sm:block hidden"> in a few easy steps.
        </h2>
        <p class="mt-5 max-w-lg {styles.paragraph}">
            Repellat aut praesentium odit velit nihil laudantium repudiandae? Neque tempore quam quos exercitationem ipsa? Quas dolore, temporibus nihil accusantium quidem quos est quae natus fugiat hic. Magni, a.
        </p>

        <Button class="mt-10" />

    </div>

    <div class="{layout.sectionImg}">
        <img src="{assetsDir + 'card.png'}" alt="Card" class="w-full h-full">
    </div>

</section>