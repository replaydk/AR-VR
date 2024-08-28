<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width, user-scalable=no, minimum-scale=1.0, maximum-scale=1.0">
        <script src="https://aframe.io/releases/1.3.0/aframe.min.js"></script>
        <!-- Import AR.js version without NFT but with marker + location-based support -->
        <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>
    </head>
    <body style="margin: 0px; overflow: hidden;">
        <a-scene embedded arjs='sourceType: webcam; debugUIEnabled: false; detectionMode: mono_and_matrix; matrixCodeType: 3x3;'>
            <!-- Marker setup to detect barcode with value '7' -->
            <a-marker type='barcode' value='7'>
                <!-- Yellow box to display when marker is detected -->
                <a-box position="0 0.5 0" color="yellow"></a-box>
            </a-marker>

            <!-- Optional: Keep the "hiro" marker if you want to use it alongside the barcode -->
            <a-marker preset="hiro">
                <!-- Example entity for the "hiro" marker -->
                <a-entity
                    position="0 0 0"
                    scale="0.05 0.05 0.05"
                    gltf-model="your-server/https://raw.githack.com/AR-js-org/AR.js/master/aframe/examples/image-tracking/nft/trex/scene.gltf">
                </a-entity>
            </a-marker>

            <!-- Camera setup for AR.js -->
            <a-entity camera></a-entity>
        </a-scene>
    </body>
</html>
