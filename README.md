TEST

<!doctype HTML>
<html>
    <head>
        <meta name="viewport" content="width=device-width, user-scalable=no, minimum-scale=1.0, maximum-scale=1.0">
        <script src="https://aframe.io/releases/0.9.0/aframe.min.js"></script>
        <script src="https://rawgit.com/jeromeetienne/AR.js/master/aframe/build/aframe-ar.min.js"></script>
    </head>
    <body style='margin: 0px; overflow: hidden;'>
        <!-- AR.js scene setup -->
        <a-scene embedded arjs='sourceType: webcam; debugUIEnabled: false; detectionMode: mono_and_matrix; matrixCodeType: 3x3;'>
            <!-- Barcode marker setup -->
            <a-marker type='barcode' value='7'>
                <!-- Yellow box to display when marker is detected -->
                <a-box position='0 0.5 0' color='yellow'></a-box>
            </a-marker>
            <!-- Camera setup for AR.js -->
            <a-entity camera></a-entity>
        </a-scene>
    </body>
</html>
