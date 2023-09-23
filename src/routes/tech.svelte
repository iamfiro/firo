<script>
    import Server from './server.svelte';
    import INFP from '../images/INFP.png'
</script>

<section id="tech">
    <div id="left">
        <div id="title">
            <span>02</span>
            <div id="divide"></div>
            <span>TECHNOLOGY</span>
        </div>
        <span id="hello">My Extensive List of<br/>Skill</span>
        <div id="category" style="margin-top: 50px; background-color: #CEF56A; border-radius: 0px 30px 0px 0px;">
            <span id="type">Frontend</span>
            <span id="stack">Svelte · Next.js · React.js · Styled-components · Vercel · Netlify · Typescript · Javascript · HTML5 · CSS3</span>
        </div>
        <div id="category" style="background-color: #E34C4E;">
            <span id="type" style="color: #fff">Backend</span>
            <span id="stack" style="color: #fff">Node.js · Express.js · Nginx · Prisma · Mysql · PlanetScale · Postman</span>
        </div>
        <div id="category" style="background-color: #837EF2;">
            <span id="type" style="color: #fff">Design / Collaboration</span>
            <span id="stack" style="color: #fff">Figma · Zeplin · Git · Github · Visual Studio Code</span>
        </div>
        <div id="category" style="background-color: #FEC3C1; border-radius: 0px 0px 0px 30px;">
            <span id="type">Etc</span>
            <span id="stack">Arduino · C · Electron · Lua · PHP · Python · Selenium</span>
        </div>
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

    #category {
        height: 100%;
        min-height: fit-content;
        background-color: #f00;
        padding: 30px 30px;
        display: flex;
        flex-direction: column;
    }

    #type {
        font-size: 35px;
        font-weight: 300;
    }

    #stack {
        font-size: 23px;
        font-weight: 700;
        margin-top: 20px;
    }
</style>