# web1
# html css hover effect





<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link href="https://fonts.googleapis.com/css?family=Monoton&display=swap" rel="stylesheet">
    <title>Document</title>
    
    
    
    
    <style>
        * {
            margin: 0%;
            padding: 0%;
        }
        
        .mainbox {
            width: 100%;
            height: 100vh;
            background: maroon;
            box-shadow: 1px 1px 15px white inset;
        }
        
        .box {
            width: 80%;
            height: 150px;
            /* border: 1px solid white; */
            position: relative;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            overflow: hidden;
        }
        
        h1 {
            width: 100%;
            height: 100%;
            position: absolute;
            top: 0;
            left: 0;
            font-size: 80px;
            text-align: center;
            text-transform: uppercase;
            line-height: 150px;
            font-family: 'Monoton', cursive;
            font-weight: lighter;
            transition: .5s;
            color: red;
            animation: goup 5s infinite;
        }
        
        @keyframes goup {
            0% {
                top: 0;
            }
            20% {
                top: -150px;
            }
            80% {
                top: -150px;
            }
            100% {
                top: -150px;
                /* opacity: 0; */
            }
        }
        
        h1::before {
            content: 'helloworld power';
            width: 100%;
            height: 100%;
            color: white;
            position: absolute;
            top: 100%;
            font-weight: lighter;
            left: 0;
        }
        
        .squre {
            width: 100px;
            height: 100px;
            position: absolute;
            top: 10%;
            left: 50%;
            transform: translateX(-50%);
            border: 1px solid white;
            /* background: white; */
        }
        
        .squre:before {
            content: '';
            width: 100%;
            height: 100%;
            position: absolute;
            border: 2px solid red;
            /* background: maroon; */
            transform: rotate(45deg);
        }
        
        p {
            width: 50%;
            height: 150px;
            position: absolute;
            bottom: 0%;
            left: 50%;
            transform: translateX(-50%);
            font-size: 20px;
            color: white;
            background: maroon;
            border: 1px solid red;
            border-bottom: none;
            text-align: center;
            padding: 20px;
            text-transform: capitalize;
            /* box-shadow: 0px 1px 5px white inset; */
            box-sizing: border-box;
        }
        
        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    </style>
    
    
    
    
</head>
<body>
    <div class="mainbox">
        <div class="box">
            <h1>helloworld power</h1>
        </div>
        <div class="squre" id="squre">
            <img src="pngword.png" alt="">
        </div>
        <p id="para">Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti ipsa aliquid eveniet illum necessitatibus quae animi, libero cupiditate nesciunt consequuntur? Atque, quia voluptatem? Fugit impedit quae officia perspiciatis reiciendis ab.</p>
    </div>
    
    
    
    
    
    
    <script>
        var x = document.getElementById('squre');
        var y = document.getElementById('para');
        
        window.onclick = function() {
            if (x.style.background == 'white') {
                x.style.background = 'none';
                y.style.background = 'maroon';
                y.style.borderColor = 'red';
                y.style.color = 'white';
            } else {
                x.style.background = 'white';
                y.style.background = 'white';
                y.style.borderColor = "white";
                y.style.color = 'maroon';
            }
        }
    </script>
    
    
    
    
</body>

</html>
