<script>
    import Navbar from "../components/navbar.svelte";
    import Video from "../components/video.svelte";
    import RecommendationSection from "../components/recommendationSection.svelte";
    import OverlayVideo from "../components/overlayVideo.svelte";
</script>

<div class="content">
    <Navbar />
    <Video />
    <OverlayVideo />
    <RecommendationSection />
</div>

<style>
    .content {
        max-width: 100vw;
        min-height: fit-content;
        display: flex;
        flex-direction: column;
        overflow-x: hidden;
    }
</style>
