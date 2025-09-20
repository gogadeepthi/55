<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style> .out{color: yellowgreen; font-weight: bold;}</style>
</head>
<body>
    <h1> keyboard Event</h1>
    <input type="text" id="input" placeholder="Type Here">
    <p id="msg" class="out"></p>
    <script>
        let input=document.getElementById("input");
        input.addEventListener("keydown", function(e){
            document.getElementById("msg").innerText="key Down: "+e.key;
        });
        input.addEventListener("keydown", function(e){
            document.getElementById("msg").innerText="key Up: "+e.key;
        });
    </script>
</body>
</html>
