<script lang="ts">
    import Student_Circle from '../images/student_circle.png';

    let password = "loading";

    const charGroups = [
		{ name: "lowercase", min: 97, max: 123},
		{ name: "uppercase", min: 65, max: 91},
		{ name: "numbers", min: 48, max: 58},
	];

    const makeRandomChar = () => {
		// A number between 1 and 4 corresponds with charGroups array above
		let charType = Math.floor(Math.random() * charGroups.length);
		// charGroups in an array of lowercase, uppercase, numbers, & symbol options
		let low = charGroups[charType].min;
		let high = charGroups[charType].max
		// Select a random number between low and high
		let number = Math.floor(Math.random() * (high - low) + low);
		return number;
	}

	const makeRandomPw = (codelength: number) => {
		let code = "";
		for(let i = 0; i <= codelength; i++) {
			let char = String.fromCharCode(makeRandomChar());     
			code += char;
		}  
		password = code;
	}
    makeRandomPw(10)
</script>

<section id="home">
    <h1 id="title">Design & Technology</h1>
    <div id="img">
        <span id="text">{password}</span>
        <span id="text">Scroll Down ...</span>
    </div>
    <img id="student" src={Student_Circle} alt="student developer">
</section>

<style>
    section {
        padding-top: 60px;
        max-width: 1600px;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    #title {
        font-size: 100px;
        font-family: 'PPNeueMontreal';
        font-weight: 300;
        margin: 0px;
        z-index: 101;
    }
    #img {
        width: 95%;
        height: 500px;
        background-position: center;
        background-size: cover;
        background-image: url('../images/abstract.jpg');
        margin-top: -35px;
        z-index: 100;
        border-radius: 20px;
        display: flex;
        align-items: flex-end;
        justify-content: space-between;
    }
    #text {
        font-family: 'PPNeueMontreal';
        font-size: 20px;
        margin: 20px 25px;
    }
    #student {
        width: 120px;
        margin-top: -60px;
        z-index: 103;
        padding: 15px;
        background-color: #fff;
        border-radius: 100px;
        animation: rotate360 25s linear infinite;
        transform-origin: 50% 50%;
    }

    @media (max-width: 970px) {
        #title {
            font-size: 80px;
        }
        #img {
            margin-top: -30px;
        }
    }

    @media (max-width: 800px) {
        #title {
            font-size: 60px;
        }
        #img {
            margin-top: -25px;
        }
    }

    @media (max-width: 600px) {
        #title {
            font-size: 50px;
        }
        #img {
            margin-top: 30px;
        }
    }

    @media (max-width: 550px) {
        #text {
            font-size: 17.5px;
        }
        #student {
            width: 80px;
        }
    }

    @media (max-width: 500px) {
        #title {
            font-size: 40px;
        }
        #text {
            font-size: 15px;
        }
        #student {
            width: 60px;
            margin-top: -40px;
        }
        #img {
            margin-top: 20px;
        }
        
    }

    @media (max-width: 400px) {
        #title {
            font-size: 30px;
        }
        #img {
            margin-top: 20px;
        }
    }

    @keyframes rotate360 {
        100% {
            transform: rotate(360deg);
        }
    }
</style>