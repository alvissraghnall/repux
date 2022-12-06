<script>
    import GetStarted from "./GetStarted.svelte";
    import styles from "../style";
    import {assetsDir} from "../constants";
</script>

<section class="flex {styles.paddingY} md:flex-row flex-col">
    <div class="flex-1 xl:px-0 sm:px-16 {styles.flexStart} flex-col px-6">
        <div class="flex flex-row items-center px-4 py-2.5 bg-discount-gradient mb-2 rounded-[10px]">
            <img src={assetsDir + "discount.svg"} alt="discount" class="w-8 h-8">
            <span class="ml-2 {styles.paragraph}">
                <span class="text-white">20%</span>
                Discount for {" "}
                <span class="text-white font-medium">1 month</span> {" "} Account
            </span> 
        </div>

        <div class="flex flex-row justify-between items-center w-full">
            <h1 class="font-poppins flex-1 font-semibold ss:text-[72px] text-[52px] text-white ss:leading-[100px] leading-[75px]">
                The Next <br class="hidden sm:block"> {" "}
                <span class="text-gradient">
                    Generation
                </span> 
            </h1>

            <div class="ss:flex md:mr-4 hidden mr-0">
                <GetStarted />
            </div>
        </div>

        <h1 class="capitalize font-poppins font-semibold w-full ss:text-6xl text-[52px] text-white ss:leading-[100px] leading-[75px]">
            payment method
        </h1>
        <p class="{styles.paragraph} max-w-md mt-5">
            Our team of experts use a methodology to identify the credit cards most likely to fit your needs. We examine annual percentage rates, and annual fees.

        </p>

    </div>

    <div class="flex flex-1 {styles.flexCenter} relative my-10 md:my-0">
        <img 
            src="{assetsDir + "robot.png"}" 
            alt=""
            class="w-full h-full relative z-[5] "
        >
        <div class="absolute h-1/3 w-2/5 top-0 pink__gradient z-0"/>
        <div class="absolute h-4/5 w-4/5 bottom-40 white__gradient z-[1]"/>
        <div class="absolute h-1/2 w-1/2 bottom-20 right-20 blue__gradient z-0"/>
    </div>

    <div class="ss:hidden {styles.flexCenter}">
        <GetStarted />
    </div>
</section>

<!-- markup (zero or more items) goes here -->