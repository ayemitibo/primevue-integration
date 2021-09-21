<template>
  <VTable :options="options">
    <template #name="{ propsItem }"> hello {{ propsItem }} </template>
    <!-- <template #status="{ propsItem }">  {{ propsItem.name }} </template> -->
  </VTable>
</template>
<script>
import VTable from "@/components/VTable";
export default {
  components: {
    VTable,
  },
  data() {
    return {
      options: [
        { title: "Name", priority: 1, field: "name" },
        { title: "Status", priority: 1, field: "status" },
        { title: "Activity", priority: 1, field: "activity" },
        { title: "Balance", field: "balance" },
      ],
    };
  },
  // setup() {

  // },
};
</script>