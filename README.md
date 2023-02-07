# varunsrepo

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Digital Clock</title>
</head>
<body>
    <h1 id="clock"></h1>
    <button onClick="stopTime()">Stop</button>
    <script>
        var intervalId = setInterval(showTime, 1000);
        var clock = document.getElementById("clock")
        
        function showTime(){
              var time = new Date()
              clock.innerHTML = `${time.getHours()}:${time.getMinutes()}:${time.getSeconds()}`
        }

        function stopTime() {
            clearInterval(intervalId)
        }
    </script>
    
</body>
</html>
