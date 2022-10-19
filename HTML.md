# HTML

>Below is a block of code used for a "**fizzbuzz**" project written in **HTML** and **Java**. 
>The **file** is also **available** in this **repository** for **download**.

>[Return](README.md)

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Fizz Buzz</title>
<script>

function fizzbuzz() {
	var display = document.getElementById('display');
	var displayHTML = "";
	for (i = 0; i < 100; i++) {
        if (i%3==0&&i%5!=0){
            displayHTML += "<p> Fizz </p>";
        }
        else if (i%5==0&&i%3!=0){
            displayHTML += "<p> Buzz </p>";
        }
        else if (i%3==0&&i%5==0) {
            displayHTML += "<p> FizzBuzz </p>";
        }
        else {
            displayHTML += "<p> None </p>";
        }
	}
    
	display.innerHTML = displayHTML
}

</script>

</head>

<body onload="fizzbuzz()">
<div id="display">

</div>
</body>

</html>
