<script>
    export let userImage;
    export let userName;
</script>

<div class="card">
    <div class="cardImage">
        <img src="{userImage}" alt="">
    </div>

    <div class="cardUserName">
        <p>{userName}</p>
    </div>
</div>

<style>
    .card {
        width: 30%;
        height: 100%;
        display: flex;
        flex-direction: column;
    }

    .cardImage {
        width: 100%;
        min-width: 100px;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .cardUserName {
        width: 100%;
        height: 20%;
        display: flex;
        justify-content: center;
        align-items: end;
    }

    .cardUserName p {
        font-size: 0.8rem;
        font-family: Sans, Helvetica Neue, Segoe UI, Roboto, Ubuntu, sans-serif;
        color: gray;
        display: flex;
    }

    .cardImage img {
        max-width: 100%;
        max-height: 70%;
        border-radius: 3%;
    }

    .cardImage img:hover {
        cursor: pointer;
        border: white 2px solid;
    }
</style>