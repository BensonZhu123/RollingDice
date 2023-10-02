
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
</head>
<script>
    function initialize(){
        nums = document.getElementById("output");
        die1 = 0
        die2 = 0
        total = 0;
    }
    function roll(){
        die1 = Math.floor((Math.random() * 6) +1);
        die2 = Math.floor((Math.random() * 6) +1);
        total = die1 + die2;
        display();
    }
    function display(){
        nums.innerHTML = "Die 1: " + die1 + "    Die 2 : " + die2 + "    Total: " + total;
    }
</script>
<body onload  = "initialize();">
    <h1 id = "output">Die 1: 0     Die 2: 0    Total: 0</h1>
    <button onclick = "roll();">Roll</button>
    
</body>
</html>
