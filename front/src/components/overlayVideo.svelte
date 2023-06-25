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
        <div class="rankVideo"></div>
        <div class="descriptionVideo">
            <p class="textDescription">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget venenatis sapien. Cras sollicitudin porta mauris, sed cursus nisi malesuada in. Etiam.</p>
        </div>
        <div class="buttonsVideo"></div>
    </div>
    <div class="ageAndSound"></div>
</div>

<style>

    @import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');
    
    .overlayVideo {
        width: 100vw;
        height: 93vh;
        background-color: pink;
        margin-top: -93vh;
        display: flex;
    }

    .videoInfo {
        width: 50%;
        height: 100%;
        background-color: powderblue;
        display: flex;
        flex-direction: column;
        margin-left: 2.5rem;
    }

    .ageAndSound {
        width: 50%;
        height: 100%;
        background-color: rebeccapurple;
        display: flex;
    }

    .ttlVideo {
        width: 60%;
        height: 50%;
        display: flex;
        background-color: aqua;
        justify-content: end;
        flex-direction: column;
    }

    .rankVideo {
        width: 60%;
        height: 10%;
        background-color: mediumseagreen;
        display: flex;
    }

    .descriptionVideo {
        width: 70%;
        height: 15%;
        background-color: mediumpurple;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .buttonsVideo {
        width: 60%;
        height: 10%;
        background-color: mediumvioletred;
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
</style>