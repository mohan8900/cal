# cal
## cal.html
```c
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style1.css">
    <title>Document</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
</head>
<style>
    body{
        background-image: url(back.png);
    }

    .cen{
        font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
        font-size: xxx-large;
        font-weight: bolder;
        height: 90%;
    }
    
</style>
<body >
    <script>
        function fn(e){
            if (e.innerHTML == '='){
                output.value = eval(output.value);
            }
            else if (e.id == 'back'){
                v=output.value;
                output.value = v.substring(0,v.length-1);
            }
            else if(e.innerHTML== 'C'){
                output.value='';
            }
            else{
                output.value += e.innerHTML;
            }
        }
    </script>
    <div class="content">
    
    <div class="row mx-auto text-center " style=" width: 24rem;background-image: url(calc_bg.jpg);background-size: cover;border-radius: 10px;">
         <div class="cen">
            <div class=" mx-auto text-center text-success" style=" width: 24rem;">Calculator</div>
        </div>
        <div class="col-12 my-4" >
            <input  type="text" name="" id="output" style=" width: 100%;height: 50px; border-radius: 25px; background: none;color: rgb(255, 254, 254);text-align: right;padding-right: 20px;">
        </div>    
    
    <div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">(</div>
    <div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">)</div>
    <div class="m-3 col-2 btn btn-danger rounded-4" onclick="fn(this)">C</div>
    <div class="m-3 col-2 btn btn-danger rounded-4" onclick="fn(this)" id="back"><i class="bi bi-backspace"></i></div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">7</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">8</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">9</div>
    <div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">*</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">4</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">5</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">6</div>
    <div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">-</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">1</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">2</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">3</div>
    <div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">+</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">0</div>
    <div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">.</div>
    <div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">%</div>
    <div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">/</div>
    <div class="m-3 col-11 btn btn-warning rounded-4" onclick="fn(this)">=</div>
    </div>
    </div>
  
    </body>
   
   
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
</body>
```
## OUTPUT:
![Screenshot 2024-07-17 223041](https://github.com/user-attachments/assets/51a8584e-2139-4960-9a08-dddbaeb962aa)
