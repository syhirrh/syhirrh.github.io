# rotating-links
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Redirecting to WhatsApp..</title>
</head>
<body>

    <script>
        var links = ["https://wa.me/601128604487", "https://wa.me/60175771517"];
        
        // Function to shuffle the links array
        function shuffleArray(array) {
            for (var i = array.length - 1; i > 0; i--) {
                var j = Math.floor(Math.random() * (i + 1));
                var temp = array[i];
                array[i] = array[j];
                array[j] = temp;
            }
            return array;
        }

        // Shuffle the links array
        shuffleArray(links);

        // Redirect to the first WhatsApp link immediately
        window.location.href = links[Math.floor(Math.random() * links.length)];
        
        // Optionally, uncomment the following lines if you want to rotate links after a delay
        // setTimeout(function() {
        //     window.location.href = links[1];
        // }, 5000); // 5000 milliseconds (5 seconds) delay
    </script>

</body>
</html>

