---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---

<html>
<head>
    <script type="text/javascript" 
	    src="https://public.tableau.com/javascripts/api/tableau-2.min.js"></script>
    <script type="text/javascript">
        function initViz() {
            var containerDiv = document.getElementById("vizContainer"),
                url = "http://public.tableau.com/views/RegionalSampleWorkbook/Storms",
                options = {
                    hideTabs: true,
                    onFirstInteractive: function () {
                        console.log("Run this code when the viz has finished loading.");
                    }
                };
            
            var viz = new tableau.Viz(containerDiv, url, options); 
            // Create a viz object and embed it in the container div.
        }
    </script>
</head>

<body onload="initViz();">

	<iframe src="https://docs.google.com/forms/d/e/1FAIpQLSdW9VL_4m0JUER5ptCy2TluF2iPfRm-bGLaUPpZbb6vVG_LSA/viewform?embedded=true" width="400" height="700" frameborder="0" marginheight="0" marginwidth="0">Loading...
	</iframe>

    <div id="vizContainer" style="width:800px; height:300px;"></div>    
</body>

</html>
