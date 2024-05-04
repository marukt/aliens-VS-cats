

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Slot Machine</title>
<style>
    .slot {
        display: inline-block;
        width: 100px;
        height: 100px;
        border: 1px solid black;
        margin: 10px;
        text-align: center;
        font-size: 24px;
        line-height: 100px;
    }
</style>
</head>
<body>
<div class="slot" id="slot1">0</div>
<div class="slot" id="slot2">0</div>
<div class="slot" id="slot3">0</div>
<button onclick="spin()">Spin</button>

<script>
    function spin() {
         var symbols = [
            'C:\Users\marilyn\Desktop\catsvsdogss\images1.png',
            'images2.png',
            'path/to/image3.png',
            'path/to/image4.png',
            'path/to/image5.png'
        ]; // Replace with your PNG image URLs or file paths

        // Generate random symbols for each slot
        var index1 = Math.floor(Math.random() * symbols.length);
        var index2 = Math.floor(Math.random() * symbols.length);
        var index3 = Math.floor(Math.random() * symbols.length);

       // Update the HTML content of each slot
        slot1.innerHTML = '<img src="' + symbols[index1] + '" alt="Symbol 1">';
        slot2.innerHTML = '<img src="' + symbols[index2] + '" alt="Symbol 2">';
        slot3.innerHTML = '<img src="' + symbols[index3] + '" alt="Symbol 3">';
    }
</script>
</body>
</html>
