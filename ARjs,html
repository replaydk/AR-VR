<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width, user-scalable=no, minimum-scale=1.0, maximum-scale=1.0">
        <script src="https://aframe.io/releases/1.3.0/aframe.min.js"></script>
        <!-- Import AR.js version without NFT but with marker + location-based support -->
        <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>
    </head>
    <body style="margin: 0px; overflow: hidden;">
        <a-scene embedded arjs>
            <!-- Marker setup to detect the custom pattern marker -->
            <a-marker type="pattern" url="https://cdn.discordapp.com/attachments/1278438301887627356/1278445377212780595/pattern-bing_generated_qrcode.patt?ex=66d0d48a&is=66cf830a&hm=48b19abbd451412db3deed287bff334bbd2940eadb56d39ad4f81e1543dc1f12&">
                <!-- Yellow box to display when marker is detected -->
                <a-box position="0 0.5 0" color="yellow"></a-box>
            </a-marker>

            <!-- Camera setup for AR.js -->
            <a-entity camera></a-entity>
        </a-scene>
    </body>
</html>
