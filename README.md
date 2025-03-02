# Javascript_Project1
### index.html
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="style.css" />
    <link rel="stylesheet" href="../styles.css" />
    <title>JavaScript Background Color Switcher</title>
  </head>
  <body>
  
    <div class="canvas">
      
      <h1>Color Scheme Switcher</h1>
      <span class="button" id="grey"></span>
      <span class="button" id="white"></span>
      <span class="button" id="deepskyblue"></span>
      <span class="button" id="yellow"></span>
      <h2>
        Try clicking on one of the colors above
        <span>to change the background color of this page!</span>
      </h2>
    </div>
    <script src="script.js"></script>
  </body>
</html>
```
### style.css
```
html {
    margin: 0;
  }
  
  span {
    display: block;
  }
  .canvas {
    margin: 100px auto 100px;
    width: 80%;
    text-align: center;
  }
  
  .button {
    width: 100px;
    height: 100px;
    border: solid black 2px;
    display: inline-block;
  }
  
  #grey {
    background: grey;
  }
  
  #white {
    background: white;
  }
  #deepskyblue {
    background: deepskyblue;
  }
  #yellow {
    background: yellow;
  }
  
```
### script.js
```
const buttons = document.querySelectorAll('.button')
const body = document.querySelector("body")

buttons.forEach(function(button){
    console.log(button);
    button.addEventListener('click',function(e){
       // console.log(e);
      //console.log(e.target);
    //   if(e.target.id=="grey"){
    //    body.style.backgroundColor = e.target.id;
    //   }
    //  else if(e.target.id=="blue"){
    //    body.style.backgroundColor = e.target.id;
    //   }
    //  else if(e.target.id=="yellow"){
    //    body.style.backgroundColor = e.target.id;
    //   }
    //   else{
    //    body.style.backgroundColor = e.target.id;
    //   }
    body.style.backgroundColor = e.target.id;
        
    });
});
```

