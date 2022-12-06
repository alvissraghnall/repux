<script>
    import styles, { layout } from "../style";
    import { assetsDir } from "../constants";
    import Button from "../shared/Button.svelte";
</script>

<section class="{styles.flexCenter} {styles.marginY} {styles.padding} box-shadow flex-col rounded-2xl sm:flex-row bg-black-gradient-2">
    <div class="flex flex-col flex-1">
        <h2 class="{styles.heading2}">Try us now!</h2>
        <p class="mt-5 max-w-lg {styles.paragraph}">
            Everything you need to accept payments & grow your business anywhere on the planet.
        </p>
    </div>
    <div class="sm:mt-0 mt-10 ml-0 sm:ml-10 {styles.flexCenter}">
        <Button />
    </div>
</section>