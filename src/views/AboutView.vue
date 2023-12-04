<template>
  <div class="about">
    <h1 class="text-2xl lg:text-3xl">This is an about page</h1>

    <div class="mt-3">
      <a-collapse v-model:activeKey="activeKey">
        <a-collapse-panel key="1" header="This is panel header 1">
          <p>{{ text }}</p>
        </a-collapse-panel>
        <a-collapse-panel key="2" header="This is panel header 2">
          <p>{{ text }}</p>
        </a-collapse-panel>
        <a-collapse-panel
          key="3"
          header="This is panel header 3"
          collapsible="disabled"
        >
          <p>{{ text }}</p>
        </a-collapse-panel>
      </a-collapse>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
}
</style>
<script setup>
import { Collapse, CollapsePanel } from "ant-design-vue";
import { ref, watch } from "vue";
const text = `A dog is a type of domesticated animal.Known for its loyalty and faithfulness,it can be found as a welcome guest in many households across the world.`;
const activeKey = ref(["1"]);
watch(activeKey, (val) => {
  console.log(val);
});

const ACollapse = Collapse;
const ACollapsePanel = CollapsePanel;
</script>
