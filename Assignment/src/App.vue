<template>
  <div class="row">
    <DraggableColumn heading="Beginning" :list="beginning" group="workspace"/>
    <DraggableColumn heading="Middle" :list="middle" group="workspace" />
    <DraggableColumn heading="End" :list="end" group="workspace" />
    <DraggableColumn heading="Idea Gallery" :list="ideaGallery" group="workspace"/>
  </div>
</template>

<script>
    import DraggableColumn from "./components/DraggableColumn.vue";

    export default {
        components: {
            DraggableColumn
        },
        data() {
            return {
                beginning: [
                    "Title",
                    "Agenda",
                    "Executive Summary",
                    "Vision",
                    "Objectives",
                    "Guiding Principles",
                    "Priorities",
                ],
                middle: [
                    "Landscape",
                    "Competitive Landscape",
                    "Profile",
                    "Product Overview",
                    "Value Preposition",
                    "Positioning",
                    "Promotions",
                    "Channel",
                    "Critical Success Factors"
                ],
                end: [
                    "Dependencies",
                    "Milestones",
                    "Resources",
                    "Risks & Benefits",
                    "What's Next",
                    "Enablement"
                ],
                ideaGallery: [
                    "Approach",
                    "Background",
                    "Context",
                    "Imperatives",
                    "Messages",
                    "People"
                ]
            };
        },
    };
</script>

<style scoped>
  .row{
    display: flex;
    justify-content: space-around;
  }
</style>
