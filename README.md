# Sum-in-js
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
