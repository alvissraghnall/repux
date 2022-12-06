<script>
    import { clients } from "../constants";
    import styles from "../style";
</script>

<section class="my-4 {styles.flexCenter}">
    <div class="{styles.flexCenter} w-full flex-wrap">
        {#each clients as client}
            <div class="flex-1 {styles.flexCenter} sm:min-w-[192px] min-w-[120px]">
                <img src="{client.logo}" alt="Client logo {client.id}" class="w-24 object-contain sm:w-48 hover:text-dimWhite">
            </div>
        {/each}
    </div>
</section>
