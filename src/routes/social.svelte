<script>
    import SpotifyArrow from '../images/spotify-arrow.png';
    import ArrowWhite from '../images/arrow-white.png';
</script>

<section id="social">
    <div id="left">
        <div style="display: flex; flex-direction: column;">
            <div id="title">
                <span>03</span>
                <div id="divide"></div>
                <span>SOCIAL</span>
            </div>
            <span id="hello">How to reach<br/>Me</span>
        </div>
        <div>
            <div id="spotifymessagewrap">
                <span id="spotifymessage">It's my favorite song</span>
                <img src={SpotifyArrow} width="15" height="15" alt="arrow" style="transform: rotate(90deg)">
            </div>
            <iframe style="border-radius:12px" title="https://open.spotify.com/embed/track/7CVYxHq1L0Z4G84jTDS6Jl?utm_source=generator" src="https://open.spotify.com/embed/track/7CVYxHq1L0Z4G84jTDS6Jl?utm_source=generator" width="100%" height="202" frameBorder="0" allowfullscreen={false} allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
        </div>
    </div>
    <div id="right">
        <a href="https://discord.com/channels/@me" target="_blank">
            <div class="socialcard" style="background-color: #5865F2;">
                <div>
                    <img src="/svg/discord.svg" width="30" alt="discord logo">
                    <img src={ArrowWhite} width="23" class="arrow" alt="arrow">
                </div>
                <div>
                    <span id="socialname">discord</span>
                    <span id="socialvalue">iam.firo</span>
                </div>
            </div>
        </a>
        <a href="mailto:mail@firos.dev" target="_blank">
            <div class="socialcard" style="background-color: #EA4335;">
                <div>
                    <img src="/svg/mail.svg" width="30" alt="mail logo">
                    <img src={ArrowWhite} width="23" height="23" class="arrow" alt="arrow">
                </div>
                <div>
                    <span id="socialname">mail</span>
                    <span id="socialvalue">mail@firos.dev</span>
                </div>
            </div>
        </a>
        <a href="https://www.instagram.com/tjdwn.firo/" target="_blank">
            <div class="socialcard" style="background-color: #E4405F;">
                <div>
                    <img src="/svg/instagram.svg" width="30" alt="instagram logo">
                    <img src={ArrowWhite} width="23" height="23" class="arrow" alt="arrow">
                </div>
                <div>
                    <span id="socialname">instagram</span>
                    <span id="socialvalue">tjdwn.firo</span>
                </div>
            </div>
        </a>
        <a href="https://github.com/firo" target="_blank">
            <div class="socialcard" style="background-color: #000;">
                <div>
                    <img src="/svg/github.svg" width="30" alt="github logo">
                    <img src={ArrowWhite} width="23" height="23" class="arrow" alt="arrow">
                </div>
                <div>
                    <span id="socialname">github</span>
                    <span id="socialvalue">iamfiro</span>
                </div>
            </div>
        </a>
    </div>
</section>

<style lang="scss">
    section {
        padding-top: 60px;
        margin-top: 150px;
        display: flex;
        width: 90%;
        min-height: fit-content;
        font-family: 'PPNeueMontreal';
        font-weight: 300;
        justify-content: space-between;
    }

    #left, #right {
        width: 45%;
        height: 100%;
        min-height: calc(100vh - 110px);
        background-color: #fff;
        display: flex;
        flex-direction: column;
    }

    #left {
        justify-content: space-between;
        #title {
            display: flex;
            align-items: center;
            span {
                font-size: 18px;
                color: rgb(0, 0, 0);
            }
            #divide {
                background-color: #cecece;
                height: 1px;
                width: 60px;
                margin: 0px 15px;
            }
        }

        #spotifymessagewrap {
            margin-bottom: 15px;
            display: flex;
            align-items: flex-end;
        }

        #spotifymessage {
            font-family: 'Nanum Hand';
            font-size: 25px;
            margin: 0px 10px 0px 15px;
        }

        #hello {
            margin-top: 20px;
            font-size: 60px;
            line-height: 50px;
        }
    }

    #right {
        min-height: calc(100vh - 210px);
        background-color: #f1f1f1;
        padding: 20px;
        border-radius: 30px;
        display: flex;
        flex-direction: column;

        .socialcard {
            padding: 20px;
            width: calc(100% - 40px);
            height: fit-content;
            border-radius: 20px;
            display: flex;
            flex-direction: column;
            margin: 10px 0px;

            div:nth-child(1) {
                display: flex;
                justify-content: space-between;
            }

            div:nth-child(2) {
                display: flex;
                flex-direction: column;
            }

            #socialname {
                color: #ffffffad;
                font-size: 19px;
                margin-top: 20px;
            }

            #socialvalue {
                font-family: 'Pretendard';
                font-weight: 500;
                font-size: 38px;
                color: #fff;
            }
        }

        .arrow {
            transform: rotate(45deg);
        }
    }
    @media (max-width: 800px) {
        section {
            flex-direction: column
        }
        #right {
            width: calc(100% - 40px);
        }

        #left {
            width: 100%;
            display: flex;
            min-height: fit-content;
            div:nth-child(2) {
                margin-top: 80px;
            }
        }
    }
    @media (max-width: 400px) {
        #right {
            width: calc(100% - 30px);
            padding: 15px;
            margin-top: -20px;
        }
        #socialvalue {
            font-size: 30px !important;
        }
    }
</style>