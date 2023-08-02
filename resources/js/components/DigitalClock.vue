<template>
    <div class="">
        <div class="w-auto lg:w-1/4 flex flex-col">
            <p class="font-bold text-white">{{ currentTime.toLocaleTimeString() }}</p>
            <p class="font-bold text-white">{{ currentTime.toLocaleDateString() }}</p>
        </div>
    </div>
</template>
<script>
import { useCurrentTime } from '../useCurrentTime';
export default {
    name: "CurrentTimeExample",
    setup() {
        const { currentTime } = useCurrentTime();
        console.log(currentTime.value);
        return { currentTime };
    },
};
</script>
