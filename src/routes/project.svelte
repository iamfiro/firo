<script>
    // @ts-ignore
    import ArrowWhite from '../images/arrow-white.png';
</script>

<section id="tech">
    <div id="left">
        <div id="title">
            <span>02</span>
            <div id="divide"></div>
            <span>PROJECT</span>
        </div>
        <span id="hello">Featured Project <span style="font-size: 40px;">🚀</span></span>

        <div id="project_container">
            <a href="https://lofi.firos.dev/" class="shadow_lofi" id="project" style="background-image: url(/src/images/lofi-station.png);">
                <div id="bottom">
                    <div>
                        <span id="project_title">Lofi Station</span>
                        <div><img src="/svg/nextdotjs-color.svg" style="filter: invert(100%)" width="20" alt="svelte"></div>
                    </div>
                    <div>
                        <span id="project_description">Easier to listen to lofi<br/></span>
                        <a href="https://lofi.firos.dev/">
                            <img style="filter: invert(100%); transform: rotate(45deg)" src={ArrowWhite} width="14" class="arrow" alt="arrow">
                        </a>
                    </div>
                </div>
            </a>
            <a href="https://github.com/iamfiro/Zandi" class="shadow_zandi" id="project" style="background-image: url(/src/images/zandi.png);">
                <div id="bottom">
                    <div>
                        <span id="project_title">Zandi</span>
                        <div><img src="/svg/electron.svg" width="20" alt="svelte"></div>
                    </div>
                    <div>
                        <span id="project_description">Check your GitHub contributions easily</span>
                        <a href="https://github.com/iamfiro/Zandi">
                            <img style="filter: invert(100%); transform: rotate(45deg)" src={ArrowWhite} width="14" class="arrow" alt="arrow">
                        </a>
                    </div>
                </div>
            </a>
        </div>
    </div>
</section>

<style lang="scss">
    section {
        display: flex;
        padding-top: 60px;
        margin-top: 100px;
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

        #project_container {
            display: flex;
            flex-wrap: wrap;
            width: 100%;
            padding: 60px 0px;
        }

        #project {
            width: 340px;
            height: 400px;
            border-radius: 20px;
            margin: 0px 20px 20px 0px;
            background-color: rgb(41, 111, 224);
            display: flex;
            align-items: flex-end;
            justify-content: center;
            box-shadow: 0 4px 16px 0 rgba(0,0,0,.04);
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            transition: all 0.4s;
            &:hover {
                cursor: pointer;
                margin-top: -20px;
                border-radius: 12px;
            }
        }

        #bottom {
            height: 75px;
            padding: 15px 20px;
            width: calc(100% - 75px);
            backdrop-filter: blur(10px);
            margin-bottom: 16px;
            border-radius: 17px;
            background-color: rgba(0, 0, 0, 0.458);
            color: #fff;
            display: flex;
            flex-direction: column;
            justify-content: space-between;

            div:nth-child(1), div:nth-child(2) {
                display: flex;
                justify-content: space-between;
                align-items: flex-end;
            }

            div:nth-child(2) {
                align-items: center;
            }

            a {
                width: 65px;
                height: 32px;
                background-color: #fff;
                border-radius: 100px;
                display: flex;
                align-items: center;
                justify-content: center;
                text-decoration: none;
                color: #000;
                font-family: 'Pretendard-Regular';
            }
        }

        #project_title {
            font-size: 22px;
            font-family: 'Pretendard-Regular';
            letter-spacing: 0.5px;
        }

        #project_description {
            font-size: 17px;
            font-family: 'Pretendard-Regular';
            letter-spacing: 0.5px;
            color: #bbb;
            max-width: 160px;
        }
    }

    @media(max-width: 700px) {
        #project_container {
            justify-content: center;
        }

        #project_container {
            justify-content: center
        }

        #project {
            margin: 0px 0px 20px 0px !important;
        }
    }
    @media(max-width: 350px) {
        #project_description {
            display: none;
        }

        #bottom {
            a {
                width: 100% !important;
            }
        }
    }

    .shadow_blue:hover {
        box-shadow: 0 10px 100px 0 #3a4be89a;
    }
    .shadow_zandi:hover {
        box-shadow: 0 10px 100px 0 #39c95bb8 !important;
    }
    .shadow_lofi:hover {
        box-shadow: 0 10px 100px 0 #702280b8 !important;
    }
</style>