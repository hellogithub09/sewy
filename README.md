<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Season Cards</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Shantell+Sans&display=swap');
        html, body{
          height: 100%;
          width: 100%;
          padding: 0;
          margin: 0;
        }

        .container {
            display: flex;
            justify-content: space-around;
            position: relative;
           
            
            height: 100%;
            width: 100%;
        }
   

        .box {
            background-color: white;
            height: 450px;
            width: 300px;
            border-top-left-radius: 30px;
            border-bottom-right-radius: 30px;
            transition: transform 1s ease;
            position: relative;
            margin-top: 100px;
        }

        .box:hover {
            transform: rotateY(180deg);
        }

        .front,
        .back {
            position: absolute;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Shantell Sans', sans-serif; /* Use Shantell Sans font */
            font-size: 40px;
            width: 100%;
            height: 100%;
        }

        .front img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-top-left-radius: 30px;
            border-bottom-right-radius: 30px;
        }

        .back {
            color: white;
            transform: rotateY(180deg);
            text-align: center;
            opacity: 0;
            transition: opacity 1s ease;
            z-index: 1;
        }

        .box:hover .back {
            opacity: 1;
        }

        .box:hover .front img {
            opacity: 0;
        }
        .autumn{
          background: rgb(40,50,40);
                background: linear-gradient(0deg, rgba(40,50,40,1) 0%, rgba(234,157,52,1) 61%);
                border-top-left-radius: 30px;
            border-bottom-right-radius: 30px;
        }
        .winter{
          background: rgb(61,66,82);
background: linear-gradient(0deg, rgba(61,66,82,1) 0%, rgba(35,54,30,1) 61%); 
border-top-left-radius: 30px;
            border-bottom-right-radius: 30px;
        }
        .spring{
          background: rgb(51,56,95);
background: linear-gradient(0deg, rgba(51,56,95,1) 0%, rgba(217,173,220,1) 61%); 
border-top-left-radius: 30px;
            border-bottom-right-radius: 30px;
        }
        .summer{
          background: rgb(23,31,24);
background: linear-gradient(0deg, rgba(23,31,24,1) 15%, rgba(40,53,174,1) 80%); 
border-top-left-radius: 30px;
            border-bottom-right-radius: 30px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="box side">
            <div class="front">
                <img src="benjamin-voros-wITd9_eDTw8-unsplash.jpg" alt="Autumn Image">
            </div>
            <div class="back autumn">
                AUTUMN
            </div>
        </div>
        <div class="box side">
            <div class="front">
                <img src="ian-keefe-OgcJIKRnRC8-unsplash.jpg" alt="Winter Image">
            </div>
            <div class="back winter">WINTER</div>
        </div>
        <div class="box side">
            <div class="front">
                <img src="redd-f-Lm5rkxzgiFQ-unsplash.jpg" alt="Spring Image">
            </div>
            <div class="back spring">SPRING</div>
        </div>
        <div class="box side">
            <div class="front">
                <img src="mohamed-nashah-kmihWgpbDEg-unsplash.jpg" alt="Summer Image">
            </div>
            <div class="back summer">SUMMER</div>
        </div>
    </div>
</body>
</html>
