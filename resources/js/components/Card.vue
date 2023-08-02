<template>
  <Card class="flex flex-col items-center justify-center">
    <div class="px-3 py-3">
      <DigitalClock />
    </div>
  </Card>
</template>

<script>
import DigitalClock from "./DigitalClock.vue";
export default {
    props: [
        'card',

        // The following props are only available on resource detail cards...
        // 'resource',
        // 'resourceId',
        // 'resourceName',
    ],
    components: {
      DigitalClock
    },
    mounted() {
    //
    },
}
</script>
