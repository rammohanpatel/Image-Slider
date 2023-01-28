# Image-Slider

//HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="imageslider.css">
    <title>Image-Slider</title>
</head>
<body>
    <div id="container">
        <div id="sliderbox">
            <img src="images/pex1.jpeg">
            <img src="images/pex3.jpeg">
            <img src="images/pex2.jpeg">
            <img src="images/pex4.jpeg">
           
        </div>

    </div>
    
</body>
</html>

//CSS


*{
    margin: 0;
    padding: 0;
}
#container{
    width:500px;
    overflow: hidden;
}

#sliderbox{
    position: relative;
    width: 2002px;
    animation-name: slideranimation;
    animation-duration: 16s;
    animation-iteration-count: infinite;

}

#sliderbox img{
    float: left; /*isse sari imagea horizontal line mein show hone lagegi*/
} 

@keyframes slideranimation{
    0%
    {
        left: 0px;
    }
     20%{
        left: 0px; /* humne 20% par isliye likha taki atleat 3.2s tak same image hi show ho otherwise 0s ke baad se hi woh doosri image par slide hone lagti*/
    } 
    25%{
        left: -500px;
    }
    45%{
        left: -500px;
    }
    50%{
        left: -1001px;
    }
    70%{
        left: -1001px;
    }
    75%{
        left: -1502px;
    }  
}
