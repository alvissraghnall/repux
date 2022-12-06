<script>
    export let feature;
    export let index;
    export let featuresLength;
    export let styles;
</script>

<div class="flex flex-row p-6 rounded-[20px] {index !== featuresLength - 1 ? 'mb-6' : 'mb-0'} feature-card">
    <div class="w-16 h-16 rounded-full bg-dimBlue {styles.flexCenter}">
        <img src={feature.icon} alt="" class="w-1/2 h-1/2 object-contain">

    </div>

    <div class="flex flex-col ml-3 flex-1">
        <h4 class="font-semibold text-white text-lg font-poppins mb-1"> {feature.title} </h4>
        <p class="font-normal text-dimWhite text-base font-poppins mb-1">{feature.content}</p>
    </div>
</div>