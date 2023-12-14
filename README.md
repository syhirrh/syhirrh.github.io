# rotating-links
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rotating Links</title>
</head>
<body>

    <p id="rotatingLink">Click here to rotate link</p>

    <script>
        var links = ["https://wa.me/60175771517", "https://wa.me/60133322039"];
        var linkIndex = 0;

        document.getElementById("rotatingLink").addEventListener("click", function() {
            window.location.href = links[linkIndex];
            linkIndex = (linkIndex + 1) % links.length;
        });
    </script>

</body>
</html>
