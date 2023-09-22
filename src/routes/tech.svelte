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
        <span id="hello">
            My Extensive List of<br/>Skill</span>
        <span id="type">strong</span>
        <div style="display: flex; flex-wrap: wrap">
            <Server svg="nextdotjs"/>
            <Server svg="prisma"/>
            <Server svg="react"/>
            <Server svg="styledcomponents"/>
            <Server svg="nodedotjs"/>
            <Server svg="typescript"/>
            <Server svg="javascript"/>
            <Server svg="html5"/>
            <Server svg="css3"/>
        </div>
        <span id="type">Good</span>
        <div style="display: flex; flex-wrap: wrap">
            <Server svg="svelte"/>
            <Server svg="electron"/>
            <Server svg="python"/>
            <Server svg="selenium"/>
            <Server svg="git"/>
            <Server svg="c"/>
            <Server svg="figma"/>
            <Server svg="mysql"/>
        </div>
        <span id="type">Other</span>
        <div style="display: flex; flex-wrap: wrap">
            <Server svg="arduino"/>
            <Server svg="php"/>
            <Server svg="lua"/>
            <Server svg="bootstrap"/>
            <Server svg="nginx"/>
            <Server svg="github"/>
            <Server svg="netlify"/>
            <Server svg="vercel"/>
            <Server svg="planetscale"/>
            <Server svg="postman"/>
            <Server svg="visualstudiocode"/>
            <Server svg="pycharm"/>
            <Server svg="ubuntu"/>
            <Server svg="windows"/>
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
        width: 95%;
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

    #type {
        font-size: 25px;
        font-weight: 700;
        margin: 20px 0px;
    }
</style>