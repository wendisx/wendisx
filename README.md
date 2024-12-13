<style>
        /*欢迎标题效果*/
       h1 {
            background: -webkit-linear-gradient(135deg,
                    #0eaf6d,
                    #ff6ac6 25%,
                    #147b96 50%,
                    #e6d205 55%,
                    #2cc4e0 60%,
                    #8b2ce0 80%,
                    #ff6384 95%,
                    #08dfb4);
            -webkit-text-fill-color: transparent;
            -webkit-background-clip: text;
            -webkit-background-size: 200% 100%;
            -webkit-animation: flowCss 20s infinite linear;
        }

        @-webkit-keyframes flowCss {
            0% {
                background-position: 0 0;
            }

            100% {
                background-position: -400% 0;
            }
        }
        h1:hover {
            -webkit-animation: flowCss 8s infinite linear;
        }

        /*隔离条*/
        .bg {
            margin: 5px;
            width: 100%;
            height: 0.5vh;
            background: linear-gradient(-45deg, #dae, #f66, #3c9, #09f, #66f);
            background-size: 200% 200%;
            animation: gradient 20s ease infinite;
        }
        @keyframes gradient {
            0% {
                background-position: 0 12%;
            }

            50% {
                background-position: 100% 100%;
            }

            100% {
                background-position: 0 12%;
            }
        }
        /*吃豆人*/
        .pacMan {
            display: inline-block;
            position: relative;
            margin: 0px;
        }
        .pacMan::before {
            content: '';
            width: 0.4em;
            height: 0.4em;
            border-radius: 50%;
            background-color: #333;
            position: absolute;
            top: 6px;
            left: 21px;
            z-index: 2000;
        }
        .mouth1 {
            width: 0;
            height: 0;
            border: 25px solid #E1B204;
            border-radius: 50%;
            border-right-color: transparent;
            animation: upup .32s 0s infinite;
            position: relative;
            z-index: 3;
        }
        @keyframes upup {
            0% {
                transform: rotate(270deg);
            }

            50% {
                transform: rotate(1turn);
            }

            100% {
                transform: rotate(270deg);
            }
        }
        .mouth2 {
            width: 0;
            height: 0;
            border: 25px solid #E1B204;
            border-right-color: transparent;
            border-radius: 25px;
            margin-top: -50px;
            animation: downdown .32s 0s infinite;
            position: relative;
            z-index: 3;
        }
        @keyframes downdown {
            0% {
                transform: rotate(90deg);
            }

            50% {
                transform: rotate(0);
            }

            100% {
                transform: rotate(90deg);
            }
        }
        .beanOne {
            background-color: #E1B204;
            border-radius: 50%;
            width: 10px;
            height: 10px;
            position: absolute;
            transform: translateY(-6px);
            top: 25px;
            left: 100px;
            animation: beanAnimation 1s linear .52s infinite;
        }

        .beanTwo {
            background-color: #E1B204;
            border-radius: 50%;
            width: 10px;
            height: 10px;
            position: absolute;
            transform: translateY(-6px);
            top: 25px;
            left: 100px;
            animation: beanAnimation 1s linear 1.1s infinite;
        }
        @keyframes beanAnimation {
            75% {
                opacity: .72;
            }

            100% {
                transform: translate(-100px, -6px);
            }
        }
        /*边框样式*/
        *{
            margin:0;
            padding:0;
        }   

        .container{  
        padding-top: 20px;
        padding-bottom: 20px;
        position: relative;
        top: 130px;
        }
        .content h2{ font-size:19px;}
        .box{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 300px;
        height: 300px;
        background: #111845a6;
        box-sizing: border-box;
        overflow: hidden;
        box-shadow: 0 20px 50px rgb(23, 32, 90);
        border: 2px solid #2a3cad;
        color: white;
        padding: 20px;
        }

        .box:before{
        content: '';
        position:absolute;
        top:0;
        left:-100%;
        width:100%;
        height:100%;
        background: rgba(255,255,255,0.1);
        transition:0.5s;
        pointer-events: none;
        }

        .box:hover:before{
        left:-50%;
        transform: skewX(-5deg);
        }


        .box .content{
        position:absolute;
        top:15px;
        left:15px;
        right:15px;
        bottom:15px;
        border:1px solid #f0a591;
        padding:20px;
        text-align:center;
        box-shadow: 0 5px 10px rgba(9,0,0,0.5);
        
        }

        .box span{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        display: block;
        box-sizing: border-box;
        
        }

        .box span:nth-child(1)
        {
        transform:rotate(0deg);
        }

        .box span:nth-child(2)
        {
        transform:rotate(90deg);
        }

        .box span:nth-child(3)
        {
        transform:rotate(180deg);
        }

        .box span:nth-child(4)
        {
        transform:rotate(270deg);
        }

        .box span:before
        {
        content: '';
        position: absolute;
        width:100%;
        height: 2px;
        background: #50dfdb;
        animation: animate 4s linear infinite;
        }

        @keyframes animate {
        0% {
        transform:scaleX(0);
        transform-origin: left;
        }
        50%
        {
            transform:scaleX(1);
        transform-origin: left;
        }
        50.1%
        {
            transform:scaleX(1);
        transform-origin: right;
            
        }
        
        100%
        {
            transform:scaleX(0);
        transform-origin: right;
            
        }
        } 
</style>

<h1>Welcome to my personal homepage 👋</h1>

<div class="pacMan">
        <div class="eye"></div>
        <div class="mouth1"></div>
        <div class="mouth2"></div>
        <div class="beanOne"></div>
        <div class="beanTwo"></div>
</div>

### 🛠 Tech Stack
<div class="bg"></div>

#### 💻Programming Language

![Golang](https://img.shields.io/badge/-Go-00ADD8?style=flat&logo=go&logoColor=white)

![Shell](https://img.shields.io/badge/-Shell-4EAA25?style=flat&logo=gnu-bash&logoColor=white)

#### ⚙️ OS

![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat&logo=linux&logoColor=black)


### 👨‍💻 About me
<div class="bg"></div>

  <div class="container">
      <div class="box">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <div class="content">
          <h2>Contact Me</h2>
          <p>
          <a>QQ:2195058149</a>
          <br/>
          <a>mail:2195058149@qq.com</a>
          </p>
        </div>
  </div>
