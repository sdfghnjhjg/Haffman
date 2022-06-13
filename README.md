<html>
<head>
    <title>
        Huffman Coding Visualization
    </title>
    <meta charset="windows-1251">
    <!-- css sheet for how the page is laid out -->
    <link rel="stylesheet" href="visualizationPageStyle.css">

    <!-- jqueury stuff.  Only used for the animation speed slider. -->
    <link rel="stylesheet" href="ThirdParty/jquery-ui-1.8.11.custom.css">
    <script src="ThirdParty/jquery-1.5.2.min.js"></script>
    <script src="ThirdParty/jquery-ui-1.8.11.custom.min.js"></script>
    <!-- Javascript for the actual visualization code -->
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/CustomEvents.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/UndoFunctions.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/AnimatedObject.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/AnimatedLabel.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/AnimatedCircle.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/AnimatedRectangle.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/AnimatedLinkedList.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/HighlightCircle.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/Line.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/ObjectManager.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AnimationLibrary/AnimationMain.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AlgorithmLibrary/Algorithm.js"></script>
    <script type="text/javascript" charset="windows-1251" src="AlgorithmLibrary/Huffman.js"></script>

</head>
<body onload="init();" class="VisualizationMainPage">
    <div id="container">
        <div id="header">
            <h1> Дерево кодирования Хаффмана</h1>
        </div>
        <div id="mainContent">
            <div id="algoControlSection">
                <!-- Table for buttons to control specific animation (insert/find/etc) -->
                <!-- (filled in by javascript code specific to the animtion) -->
                <table id="AlgorithmSpecificControls">
             
                </table>
            </div>
            <!-- Drawing canvas where all animation is done.  Note:  can be resized in code -->
            <canvas id="canvas" width="1000" height="516"></canvas>
            <div id="generalAnimationControlSection">
                <!-- Table for buttons to control general animation (play/pause/undo/etc) ->
                <!-- (filled in by javascript code, specifically AnimationMain.js)  -->
                <table id="GeneralAnimationControls">  </table>
            </div>
        </div> <!-- mainContent -->
        <!--
        <!<div id="footer">
            <p><a href="Algorithms.html">Algorithm Visualizations</a></p>
        </div> -->

    </div><!-- container -->
</body>
</html>
