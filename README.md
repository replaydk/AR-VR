<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width, user-scalable=yes, minimum-scale=1.0, maximum-scale=1.0">
        <script src="https://aframe.io/releases/1.3.0/aframe.min.js"></script>
        <!-- Import AR.js version without NFT but with marker + location-based support -->
        <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>
    </head>
    <body style="margin: 0px; overflow: hidden;">
        <a-scene embedded arjs>
            <!-- Marker setup to detect the custom pattern marker -->
            <a-marker type="pattern" url="https://github.com/replaydk/AR-VR/blob/main/pattern-bing_generated_qrcode.patt">
                <!-- Yellow box to display when marker is detected -->
                <a-box position="0 0.5 0" color="yellow"></a-box>
            </a-marker>

            <!-- Camera setup for AR.js -->
            <a-entity camera></a-entity>
        </a-scene>
    </body>
</html>
