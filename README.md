<!DOCTYPE html>
<html>
<head>
    <title>Your Website Name</title>
</head>
<body>
    <!-- Connect Button -->
    <button id="connectButton">Connect US</button>

    <!-- List Display -->
    <ul id="connectList">
        <li><a href="https://t.me/hanif_crypto_2580">Tellegram</a></li>
        <li><a href="https://www.facebook.com/hanif884401">Facebook page</a></li>
        <li><a href="https://www.youtube.com/@mdabuhanif2501">YouTube channel</a></li>
        <li>WhatsApp number: +8801704625884</li>
    </ul>

    <!-- JavaScript Code -->
    <script>
        // Click event handler for the Connect Button
        document.getElementById('connectButton').addEventListener('click', function() {
            // Toggle class to show/hide the list
            var connectList = document.getElementById('connectList');
            connectList.classList.toggle('show');
        });
    </script>
</body>
</html>