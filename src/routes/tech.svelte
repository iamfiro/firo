<section id="tech">
    <div id="left">
        <div id="title">
            <span>02</span>
            <div id="divide"></div>
            <span>TECHNOLOGY</span>
        </div>
        <span id="hello">My Extensive List of<br/>Skill <span style="font-size: 40px;">😋</span></span>
        <div id="stackWrap" style="padding: 40px 0px; display: flex; flex-wrap: wrap; margin-left: -10px;">
            <div id="stack">
                <img src="/svg/svelte-color.svg" alt="svelte">
            </div>
            <div id="stack">
                <img src="/svg/nextdotjs-color.svg" alt="nextjs">
            </div>
            <div id="stack">
                <img src="/svg/react-color.svg" alt="react">
            </div>
            <div id="stack">
                <img src="/svg/nodedotjs-color.svg" alt="svelte">
            </div>
            <div id="stack">
                <img src="/svg/typescript-color.svg" alt="typescript">
            </div>
            <div id="stack">
                <img src="/svg/mysql-color.svg" alt="mysql">
            </div>
            <div id="stack">
                <img src="/svg/git-color.svg" alt="git">
            </div>
            <div id="stack">
                <img src="/svg/figma-color.svg" alt="figma">
            </div>
        </div>
        <span id="elseStack">C / ELECTRON / LUA / NGINX / PHP / PRISMA / PYTHON / STYLED-COMPONENTS / UBUNTU / ARDUINO / HTML5 / CSS3 / JAVA</span>
    </div>
    
</section>

<style lang="scss">
    section {
        display: flex;
        padding-top: 60px;
        margin-top: 20px;
        width: 90%;
        min-height: fit-content;
        font-family: 'PPNeueMontreal';
        font-weight: 300;
        justify-content: space-between;
    }

    #left {
        width: 100%;
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
    }

    #stack {
        width: 140px;
        height: 140px;
        margin: 10px 15px;
        display: flex;
        align-items: center;
        justify-content: center;
        border: 2px solid #000;
        img {
            width: 80px;
            height: 80px;
        }
    }

    #elseStack {
        margin-top: 20px;
        font-size: 45px;
        line-height: 50px;
        font-weight: 700;
    }

    @media(max-width: 1000px) {
        #elseStack {
            font-size: 40px;
        }
    }

    @media(max-width: 600px) {
        #elseStack {
            line-height: 40px;
            font-size: 30px;
        }
        #stackWrap {
            justify-content: center;
        }
        #stack {
            width: 110px;
            height: 110px;
            img {
                width: 50px;
                height: 50px;
            }
        }
    }
</style>