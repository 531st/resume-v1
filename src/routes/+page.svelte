<script>
    import ScrollTop from "../components/ScrollTop.svelte";
    import gitIcon from "../lib/assets/icons/git.png"
    import tgIcon from "../lib/assets/icons/telegram.png"
    import mailIcon from "../lib/assets/icons/gmail.png"
</script>

<div class="container">
    <div class="header">
        <p class="title neon">Meet Goshan</p>
        <div class="nav">
            <a class="nav-elem" href="#about">about</a>
            <a class="nav-elem" href="#specializations">specializations</a>
            <a class="nav-elem" href="#stack">stack</a>
            <a class="nav-elem" href="#contact">contact</a>
        </div>
    </div>
    <div class="main-body">

        <p class="para-header" id="about">About</p>
        <div class="text-block">
            <div class="text">
                Graduated from St. Petersburgs Petrovskiy college, famous for its ahead of time IT studying practices also known as Russian MIT. 
                Seasoned with working experience in MIA IT & cyber security structures and "P&G" SS Leader position.
            </div>
            <img class="img" src="https://imagedelivery.net/9sCnq8t6WEGNay0RAQNdvQ/UUID-cl9g0t3wf4954qtovbwtilgvi/public" alt="error">
        </div>

        <p class="para-header" id="specializations">Specializations</p>           
        <div class="text-block">
            <img class="img" src="https://external-preview.redd.it/a-cyberpunk-cat-hacker-is-surrounded-by-neon-lights-in-an-v0-b2uRHZzMMLj4U6C5b9_mWvwjJP1pvT-rSS5OaIxZR90.png?auto=webp&s=adcd979d483f549ed637f052a779e3adeaaa1088" alt="error">
            <p class="text left"> 
                Prepare to be blown away by the ultimate tech virtuoso! Behold a master of system administration, an unstoppable force in info sec and cybersec
                , a wizard of front-end and back-end development, a maestro of network ops, a guru of server hardware, and a genius of PC software. 
                This extraordinary individual possesses an unrivaled skill set that will leave you in awe. Experience impenetrable system security,
                 mesmerizing website functionality, flawless network operations, and mind-blowing hardware and software solutions. 
                Brace yourself for a tech revolution with our unparalleled expert leading the way!
            </p>
        </div>

        <p class="para-header" id="stack">Stack</p>
        <div class="text-block">
            <p class="text">    
                <strong>Back-end:</strong> Django, flask , PostgreSQL, MySQL, SQLite<br>
                <strong>Front-end:</strong> Svelte, and basically everything else out there, i am quick to adopt new tech!<br>
                <strong>DevOps:</strong> Docker, Git, Teraform, AWS Kubernetes, Ansible<br>
                <small><i>*Not everything is true at the moment of resume creation</i></small>
            </p>
            <img class="img" src="https://plus.unsplash.com/premium_photo-1661963212517-830bbb7d76fc?q=80&w=1986&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="error">
        </div>

        <p class="para-header" id="contact">Contact Me</p> 
        <div class="contact-block">
            <div class="contact-info">
                <div class="contact-row">
                    <img class="icon" src={gitIcon} alt="error" href="https://github.com/531st">
                    <a class="link" href="https://github.com/531st">github.com/531st</a>
                </div>
                <div class="contact-row">
                    <img class="icon" src={tgIcon} alt="error" href="https://t.me/ElDespicable">
                    <a class="link" href="https://t.me/ElDespicable">@ElDespicable</a>
                </div>
                <div class="contact-row">
                    <img class="icon" src={mailIcon} alt="error" href="mailto:sasface88@gmail.com">
                    <a class="link" href="mailto:sasface88@gmail.com">sasface88@gmail.com</a>
                </div>
            </div>
        </div>
    </div>
    <ScrollTop showAtPixel={100} />
</div>

<style>
    .container {
        display: flex;
        flex-direction: column;
        height: 100%;
    }

    .header {
        display: flex;
        flex-direction: row;
        margin-bottom: 6rem;
    }

    .title {
        font-family: 'Tilt Neon', sans-serif;
        font-size: 3rem;
        font-weight: 700;
        margin-top: 5px;
        margin-left: 15px;
        border: 0.2rem solid #fff;
        border-radius: 2rem;
        padding: 0.4em;
        box-shadow: 0 0 .2rem #fff,
                    0 0 .2rem #fff,
                    0 0 2rem #bc13fe,
                    0 0 0.8rem #bc13fe,
                    0 0 2.8rem #bc13fe,
                    inset 0 0 1.3rem #bc13fe;
    }

    .nav{
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        gap:0.8rem;
        margin-left: 2rem;
        margin-top:3rem;
    }

    .nav-elem{
        color: #FE00FB;
        font-size: 1.5rem;
        font-family: 'Tilt Neon', sans-serif;
        text-decoration: none;
    }

    .nav-elem:hover{
        color:#69FFB9;
    }

    .main-body{
        display: flex;
        flex-direction: column;
        margin-bottom: 55px;
        overflow: auto;
    }

    .text-block{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        color: white;
        font-size: 1.7vw;
        margin-left: 5rem;
        margin-right: 2rem;
        width: 85vw;
        margin-bottom: 16vh;
        gap:30px;
    }

    .text {
        width: 45vw;
        color: #949494;
    }

    .left{
        text-align: end; 
    }

    .para-header{
        margin-left: 5rem;
        color: #69FFB9;
        font-size: 1.8vw;
    }

    .img{
        height: 20rem;
        width: 20rem;
        margin-top: 1rem;
        border-radius: 3px;
        opacity: 60%;
        box-shadow: 0 0 3px #FE00FB,
            0 0 5px #FE00FB,
            0 0 7px #FE00FB,
            0 0 2px #FE00FB,
            0 0 55px #FE00FB;;
    }

    .contact-block{
        display: flex;
        flex-direction: row;
        margin-left: 5rem;
    }

    .contact-info{
        display: flex;
        flex-direction: row;
        width:85vw;
        justify-content: space-between;
    }

    .contact-row{
        display: flex;
        flex-direction: row;
        gap: 1rem;
        flex-wrap: wrap;
    }

    .icon{
        height: 3rem;
        
    }

    .link{
        font-size:2rem;
        color: yellow;
        text-decoration: none;
    }

    .neon{
        animation: flicker-green 1.5s infinite alternate;
        color: #69FFB9;
        text-shadow:
            0 0 7px #fff,
            0 0 10px #fff,
            0 0 21px #fff,
            0 0 42px #A1FADD,
            0 0 82px #A1FADD,
            0 0 92px #A1FADD,
            0 0 102px #A1FADD,
            0 0 151px #A1FADD;
    }

    .neon:hover {
        animation: flicker-pink 1.5s infinite alternate;
        color: #FE00FB;
        text-shadow:
            0 0 7px #fff,
            0 0 10px #fff,
            0 0 21px #fff,
            0 0 42px #FE00FB,
            0 0 82px #FE00FB,
            0 0 92px #FE00FB,
            0 0 102px #FE00FB,
            0 0 151px #FE00FB;
    }

    @keyframes flicker-green {
        0%, 18%, 22%, 25%, 53%, 57%, 100% {
        text-shadow:
        0 0 4px #fff,
        0 0 11px #fff,
        0 0 19px #fff,
        0 0 40px #0fa,
        0 0 80px #0fa,
        0 0 90px #0fa,
        0 0 100px #0fa,
        0 0 150px #0fa;
        }
        20%, 24%, 55% {       
            text-shadow: none;
        }
    }

    @keyframes flicker-pink {
        0%, 18%, 22%, 25%, 53%, 57%, 100% {
        text-shadow:
        0 0 4px #fff,
        0 0 11px #fff,
        0 0 19px #fff,
        0 0 40px #FE00FB,
        0 0 80px #FE00FB,
        0 0 90px #FE00FB,
        0 0 100px #FE00FB,
        0 0 150px #FE00FB;
        }
        20%, 24%, 55% {       
            text-shadow: none;
        }
    }

    @keyframes pulsate-green {
        100% {
            /* Larger blur radius */
            text-shadow:
            0 0 4px #fff,
            0 0 7px #fff,
            0 0 15px #fff,
            0 0 35px rgba(0, 255, 170, 0.149),
            0 0 75px rgba(0, 255, 170, 0.149),
            0 0 85px rgba(0, 255, 170, 0.149),
            0 0 100px rgba(0, 255, 170, 0.149),
            0 0 125px rgba(0, 255, 170, 0.149);
        }
        0% {
            /* Smaller blur radius */
            text-shadow:
            0 0 4px #fff,
            0 0 10px #fff,
            0 0 18px #fff,
            0 0 38px rgba(0, 255, 170, 0.149),
            0 0 73px rgba(0, 255, 170, 0.149),
            0 0 80px rgba(0, 255, 170, 0.149),
            0 0 94px rgba(0, 255, 170, 0.149),
            0 0 100px rgba(0, 255, 170, 0.149);
        }
    }

    @keyframes pulsate-pink {
        100% {
            /* Larger blur radius */
            text-shadow:
            0 0 4px #fff,
            0 0 11px #fff,
            0 0 19px #fff,
            0 0 40px #FE00FB,
            0 0 80px #FE00FB,
            0 0 90px #FE00FB,
            0 0 100px #FE00FB,
            0 0 150px #FE00FB;
        }
        0% {
            /* Smaller blur radius */
            text-shadow:
            0 0 2px #fff,
            0 0 4px #fff,
            0 0 6px #fff,
            0 0 10px #FE00FB,
            0 0 45px #FE00FB,
            0 0 55px #FE00FB,
            0 0 70px #FE00FB,
            0 0 80px #FE00FB;
        }
    }
</style>