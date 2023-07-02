<script>

</script>

<div class="overlayVideo">
    <div class="videoInfo">
        <div class="ttlVideo">
            <div class="firstWordBox">
                <p class="firstWord">Varius</p>
            </div>
            <div class="anotherWordsBox">
                <div class="middleWordsBox">
                    <div class="topWord">
                        <p>sit</p>
                    </div>
                    <div class="bottomWord">
                        <p>nec</p>
                    </div>
                </div>
                <div class="lastWordBox">
                    <p class="lastWord">lorem</p>
                </div>
            </div>
        </div>
        <div class="rankVideo">
            <div class="squareRank">
                <p class="txtSquareRank">Top 10</p>
            </div>
            <p class="txtRank">#1 in TV Shows Today</p>
        </div>
        <div class="descriptionVideo">
            <p class="textDescription">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget venenatis sapien. Cras sollicitudin porta mauris, sed cursus nisi malesuada in. Etiam.</p>
        </div>
        <div class="buttonsVideo">
            <div class="btnPlayBox">
                <button class="btnPlay">
                    <i class="fas fa-play"></i>
                    <p class="play">Play</p>
                </button>
            </div>
            <div class="btnInfoBox">
                <button class="btnInfo">
                    <i class="fas fa-info-circle"></i>
                    <p class="moreInfoBtn">More Info</p>
                </button>
            </div>
        </div>
    </div>
    <div class="ageAndSound">
        <div class="contentAgeAndSound">
            <div class="sound">
                <i class="fas fa-volume-mute"></i>
            </div>
            <div class="ageBox">
                <div class="ageTip"></div>
                <div class="ageSquare">
                    <p class="age">18</p>
                </div>
            </div>
        </div>
    </div>
</div>

<style>

    @import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');
    
    .overlayVideo {
        width: 100vw;
        height: 93vh;
        margin-top: -93vh;
        display: flex;
    }

    .videoInfo {
        width: 50%;
        height: 100%;
        display: flex;
        flex-direction: column;
        margin-left: 2.5rem;
    }

    .ageAndSound {
        width: 50%;
        height: 85%;
        display: flex;
        justify-content: end;
        align-items: end;
    }

    .ttlVideo {
        width: 60%;
        height: 50%;
        display: flex;
        justify-content: end;
        flex-direction: column;
    }

    .rankVideo {
        width: 60%;
        height: 10%;
        display: flex;
        align-items: center;
    }

    .descriptionVideo {
        width: 70%;
        height: 15%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .buttonsVideo {
        width: 60%;
        height: 10%;
        display: flex;
    }

    .firstWordBox {
        width: 100%;
        height: 35%;
        display: flex;
        align-items: center;
    }

    .anotherWordsBox {
        width: 100%;
        height: 35%;
        display: flex;
    }

    .middleWordsBox {
        width: 30%;
        height: 100%;
        display: flex;
        flex-direction: column;
        display: flex;
    }

    .lastWordBox {
        width: 70%;
        height: 100%;
        display: flex;
        align-items: center;
    }

    .topWord {
        width: 100%;
        height: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .bottomWord {
        width: 100%;
        height: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    p {
        font-size: 5em;
        color: white;
        font-family: 'Playfair Display', serif;
    }

    .firstWord {
        font-size: 12em;
    }

    .lastWord {
        font-size: 9em;
    }

    .textDescription {
        font-size: 1.7em;
    }

    .btnPlayBox {
        width: 35%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .btnInfoBox {
        width: 40%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    button {
        border: none;
        width: 90%;
        height: 80%;
        display: flex;
        border-radius: 5%;
    }

    .btnPlay {
        background-color: white;
        justify-content: center;
        align-items: center;
    }

    .btnInfo {
        background-color: rgb(143, 143, 143);
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .play, .moreInfoBtn {
        font-size: 1.3em;
        color: black;
    }

    button i {
        font-size: 1.5em;
        margin-right: 0.7rem;
    }

    .contentAgeAndSound {
        width: 25%;
        height: 7%;
        display: flex;
        align-items: center;
    }

    .sound {
        width: 20%;
        height: 90%;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 100%;
        border: 1px solid white;
        color: white;
        margin-right: 1rem;
    }

    .ageBox {
        width: 70%;
        height: 100%;
        display: flex;
        background-color: rgb(65, 65, 65);
        align-items: center;
    }

    .ageTip {
        width: 3%;
        height: 90%;
        background-color: white;
        display: flex;
    }

    .ageSquare {
        width: 28%;
        height: 82%;
        display: flex;
        background-color: black;
        margin-left: 1rem;
        justify-content: center;
        align-items: center;
        border-radius: 10%;
    }

    .age {
        font-size: 2em;
    }

    .squareRank {
        width: 9%;
        height: 65%;
        display: flex;
        background-color: red;
        justify-content: center;
        align-items: center;
        text-align: center;
        border-radius: 10%;
    }

    .txtRank {
        font-size: 3em;
        margin-left: 1rem;
    }

    .txtSquareRank {
        font-size: 1.3em;
    }

</style>