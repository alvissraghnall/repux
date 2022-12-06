<script>
    import { stats } from "../constants/index";
    import styles from "../style";

</script>


<section class="flex-row flex-wrap {styles.flexCenter} mb-6 sm:mb-20">
    {#each stats as stat,index}
        <div class="flex-1 justify-start items-center flex-row flex m-3">
            <h4 class="text-white text-3xl xs:leading-[50px] xs:text-4xl font-semibold font-poppins">
                {stat.value}
            </h4>
            <p class="text-base xs:text-xl font-normal font-poppins text-gradient ml-3 uppercase">
                {stat.title}
            </p>

        </div>

    {/each}
</section>