# Sum-in-js
<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Document</title>

    <link rel="stylesheet" href="style.css">

    

</head>

<body>



    <form >

        <label for="num1">number 1 : </label>

        <input id="num1" type="number"><br>

        <br>



        <label for="num2">number 2 : </label>

        <input id="num2" type="number"><br>

        <br>

    

        <button id="submitbtn">Add</button>

        <button id="subbtn">Sub</button>

        <button id="submitbtn">Product</button>



    </form>



    <div class="" id="output">Answer</div>

  

 <script src="./app.js"></script>    

</body>

</html>
//fetch buttons instances
const submitbtn = document.getElementById("submitbtn")
const output=document.getElementById("output")

//connect event to submit button (what should happen if button is clicked)
submitbtn.addEventListener("click", function show(e){
    e.preventDefault()
    //fetch number values
    const num1 = document.getElementById("num1").value
    const num2 = document.getElementById("num2").value

    //calculate sum
    let sum = Number(num1)+Number(num2)
    //display sum in html
    output.innerText="Sum is "+sum
})
