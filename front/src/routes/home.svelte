<script>
    import Navbar from "../components/navbar.svelte";
    import Video from "../components/video.svelte";
    import RecommendationSection from "../components/recommendationSection.svelte";
</script>

<div class="content">
    <Navbar />
    <Video />
    <RecommendationSection />
</div>

<style>
    .content {
        max-width: 100vw;
        min-height: fit-content;
        background-color: green;
        display: flex;
        flex-direction: column;
        overflow-x: hidden;
    }
</style>
