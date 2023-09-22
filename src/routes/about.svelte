<script>
    import { Kr } from 'svelte-flag-icons';
    import INFP from '../images/INFP.png'
</script>

<section>
    <div id="left">
        <div id="title">
            <span>01</span>
            <div id="divide"></div>
            <span>ABOUT</span>
        </div>
        <span id="hello">Hello, I'm<br/>FIRO
            <img src = "https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width=40px alt="hello">
        </span>
        <span id="description">I'm a middle school student living in <span style="font-weight: 300;">South Korea</span>,<br/>
            and I'm passionate about using development to create positive impacts. I specialize in <span style="font-weight: 300;">crafting user-centered</span>, engaging digital experiences. As a developer, I translate these principles into efficient, <span style="font-weight: 300;">user-friendly solutions that resonate with users on a meaningful level</span>.</span>
    </div>
    <div id="right">
        <article id="whereiskorea">
            <div style="display: flex; justify-content: space-between; align-items: center;">
                <span class="title">I live in South Korea :)</span>
                <Kr size={40}/>
            </div>
            <a href="https://www.google.com/maps/place/%ED%95%9C%EA%B5%AD/" target="_blank">
                <button class="koreabutton">Where is the South Korea?!</button>
            </a>
        </article>
        <article id="ilikeblue">
            <div style="display: flex; justify-content: space-between; align-items: center;">
                <span class="title">I like blue-based colors</span>
                <div id="bluecircle"></div>
            </div>
        </article>
        <article id="infp">
            <div style="display: flex; justify-content: space-between; align-items: center;">
                <span class="title">I am INFP</span>
                <span style="color: #ffffff90">yeah... it's me</span>
            </div>
            <img src={INFP} width="100%" style="margin-top: 20px; border-radius: 10px" alt="INFP Email meme">
        </article>
        <a href="https://bit.ly/3ukB4Za" target="_blank" style="width: calc(100% - 40px); max-width: 350px; margin-right: 20px;">
            <button id="magicbutton">Would you like to press it?</button>
        </a>
    </div>
</section>

<style lang="scss">
    section {
        display: flex;
        margin-top: 80px;
        width: 90%;
        min-height: 100vh;
        font-family: 'PPNeueMontreal';
        font-weight: 300;
        justify-content: space-between;
    }

    #left, #right {
        width: 45%;
        height: 100%;
        background-color: #fff;
        display: flex;
        justify-content: space-between;
        flex-direction: column;
    }

    #left {
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

        #hello {
            margin-top: 20px;
            font-size: 60px;
            line-height: 50px;
        }

        #description {
            font-weight: 700;
            margin-top: 30px;
            font-size: 19px;
            line-height: 33px;
        }
    }

    #right {
        align-items: flex-end;
        article {
            width: calc(100% - 40px);
            height: fit-content;
            max-width: 350px;
            border-radius: 15px;
            padding: 20px;
        }

        #whereiskorea {
            padding: 15px 20px 20px 20px;
            background-color: #D6FF3C;
            .title {
                font-size: 20px;
                color: #191919;
            }
            a > button {
                width: 100%;
                background-color: #191919;
                border-radius: 100px;
                height: 48px;
                border: 0px;
                margin-top: 10px;
                color: #fff;
                transition: .2s all;
                &:hover {
                    transform: scale(1.03);
                    cursor: pointer;
                }
            }
        }

        #ilikeblue {
            margin-top: 20px;
            padding: 15px 20px 20px 20px;
            background-color: #0f74f8;
            border: 1.5px solid #0f74f86b;
            .title {
                font-size: 20px;
                color: #fff;
            }
        }

        #infp {
            margin-top: 20px;
            padding: 15px 20px 20px 20px;
            background-color: #9b0ff8;
            border: 1.5px solid #9b0ff880;
            .title {
                font-size: 20px;
                color: #fff;
            }
        }
    }

    #bluecircle {
        width: 100px;
        height: 20px;
        border-radius: 5px;
        background: linear-gradient(to right, #0f74f8 40%, #fff);
    }

    #magicbutton {
        width: 100%;
        background-color: #191919;
        border-radius: 100px;
        height: 48px;
        border: 0px;
        margin-top: 30px;
        color: #fff;
        transition: .2s all;
        &:hover {
            transform: scale(1.03);
            cursor: pointer;
        }
    }
</style>