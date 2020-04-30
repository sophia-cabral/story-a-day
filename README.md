<!DOCTYPE html>
<html lang="en">
<head>

    <!-- Basic Page Needs
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <meta charset="utf-8">
    <title>Chocolate website</title>
    <meta name="description" content="">
    <meta name="author" content="">

    <!-- Mobile Specific Metas
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- FONT
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <link href="//fonts.googleapis.com/css?family=Raleway:400,300,600" rel="stylesheet" type="text/css">

    <!-- CSS
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <link rel="stylesheet" href="css/normalize.css">
    <link rel="stylesheet" href="css/skeleton.css">

    <!-- Favicon
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <link rel="icon" type="image/png" href="images/favicon.png">
    <style>

        #lottie {
            background-color: #fff;
            width: 100%;
            height: 80%;
            display: block;
            overflow: hidden;
            transform: translate3d(0,0,0);
            /*display:none;*/
        }
    </style>
</head>

<body>

    <!-- Primary Page Layout
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <header class="container example grid">
        <div class="row">
            <div class="eight columns">
                <h6><u>Sophia's daily reads</u></h6>
            </div>
            <div class="four columns" style="background-color: #FF5733">
                Story one
            </div>
        </div>
    </header>
    <div class="container example grid">
        <div class="row">
            <div class="twelve columns"><h6><i>The following is an excerpt from the book "Invisible Cities" by Italo Calvino</i></h6></div>
        </div>
    </div>

    <div class="container example grid">
        <div class="row">
            <div class="twelve" style="margin-top:15%"></div>
            <script src="lottie.js"></script>

            <div id="lottie"></div>

            <script>
                var anim;
                var elem = document.getElementById('lottie');
                var animData = {
                    container: elem,
                    renderer: 'svg',
                    loop: true,
                    autoplay: true,
                    rendererSettings: {
                        progressiveLoad: true,
                        preserveAspectRatio: 'xMidYMid meet',
                        imagePreserveAspectRatio: 'xMidYMid meet',
                        title: 'TEST TITLE',
                        description: 'TEST DESCRIPTION',
                        filterSize: {
                            width: '300%',
                            height: '300%',
                            x: '-100%',
                            y: '-100%',
                        }
                    },
                    path: 'data.json'
                };
                // lottie.setQuality('low');
                anim = lottie.loadAnimation(animData);
                // anim.setSubframe(false);
                anim.onError = function (errorType, nativeError, errorProps) {
                    console.log(errorType)
                }

                anim.addEventListener('error', function (error) {
                    console.log(error)
                })</script>
        </div>
    </div>

    <div class="container example grid">
        <div class="row">
            <div class="eight columns" >
                <a class="button" href="index4.html" target="_blank">
                    Dive in
                </a>
            </div>
        </div>
    </div>



    <!-- End Document style="background-color: #5D6D7E" style="background-color: #FF5733">
      –––––––––––––––––––––––––––––––––––––––––––––––––– -->
</body>


</html>
