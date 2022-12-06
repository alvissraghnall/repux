<script>
    import styles from "../style";
    import { assetsDir } from "../constants";
</script>


<div class="{styles.flexCenter} w-36 h-36 rounded-full bg-blue-gradient p-0.5 cursor-pointer">
    <div class="flex-col {styles.flexCenter} rounded-full h-full w-full bg-primary flex-col">
        <div class="flex-row {styles.flexStart}">
            <p class="font-poppins font-medium text-lg leading-6">
                <span class="text-gradient">
                    Get
                </span>
            </p>
            <img 
                    src="{assetsDir + "arrow-up.svg"}"
                    class="w-6 h-6 object-contain"    
                    alt="Arrow Up"
                >
        </div>

        <p class="font-poppins font-medium text-lg leading-6">
            <span class="text-gradient">
                Started
            </span>
        </p>
    </div>

</div>