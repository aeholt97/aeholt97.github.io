<!doctype html>
<head>
    <link rel="stylesheet" href="read.css"/>
    <title>Filosofisk  Debatforum</title>
    <style>
        .button {
        background-color: #90c7c5;
        border: none;
        color: white;
        padding: 10px 10px;
        text-align: center;
        height: 80px;
        text-decoration: none;
        display: block;
        font-size: 20px;
        margin: 4px 2px;
        cursor: pointer;
        }
        .buttonSC {
        background-color: #2e1bbc;
        border: none;
        color: white;
        padding: 10px 10px;
        text-align: center;
        height: 80px;
        text-decoration: none;
        display: block;
        font-size: 20px;
        margin: 4px 2px;
        cursor: pointer;
        }
        .headline {
        color: black;
        font-size: 20px;
        }
        .para {
        color: black;
        font-size: 50;
        }
         .button3 {
        background-color: #90c7c5;
        border: none;
        color: white;
        padding: 10px;
        text-align: center;
        height: 50px;
        width: 200px;
        text-decoration: none;
        font-size: 30px;
        margin: 4px 2px;
        cursor: pointer;
        }
        .button4 {
        background-color: #90c7c5;
        border: none;
        color: white;
        padding: 10px;
        text-align: center;
        height: 50px;
        width: 200px;
        text-decoration: none;
        font-size: 20px;
        margin: 4px 2px;
        cursor: pointer;
        }
        .goto {
        background-color: #90c7c5;
        border: none;
        color: white;
        padding: 10px;
        text-align: center;
        vertical-align: middle;
        height: 20px;
        text-decoration: none;
        display: inline-block;
        font-size: 15px;
        cursor: pointer;
        }
    </style>
    <script type="text/javascript" src="http://code.jquery.com/jquery-1.9.1.js"></script>
    <script>
      var locations = ["KogSem/CSkg1.pdf", "KogSem/CSkg2.pdf", "KogSem/CSkg3.pdf","KogSem/CSkg4.pdf", "KogSem/CSkg5.pdf", "KogSem/CSkg6.pdf", "KogSem/CSkg7.pdf", "KogSem/CSkg8.pdf", "KogSem/CSkg9.pdf", "KogSem/CSkg11.pdf", "KogSem/CSkg12.pdf"];
      var currentIndex = 0;
      var len = locations.length;
      $(document).ready(function(){
        $(':button').click(function() {
            currentIndex = this.value == "Next" ? 
                    currentIndex < len - 1 ? ++currentIndex : len - 1 : 
                    currentIndex > 0 ? --currentIndex : 0;
            $('#frame').attr('src', locations[currentIndex]);
        });
      });
    </script>

</head>

<div class="container">
    <div id="content1">
        <div id="nested2">
            <a class="button" href="readSC.html">Social Cognition Course</a></div>
        <div id="nested3">
            <a class="buttonSC" href="readCS.html">Cognitive Semiotics Course</a></div>
    </div>
    <div id="content3">
        <div id="nested1"><br>
            <input class="button3" type = "button" value = "Previous"/>
        </div>
        <div id="nested2">
            <p class="para"><br>Go to:</p>
            <a class="goto" href = "readCSpp.html">slides / Power points</a>
        </div>
        <div id="nested3"> <br>
            <input class="button3" type = "button" value = "Next"/>
        </div>    
    </div><br>
    <div id="content4">
        <div id="nested"></div>
        <div id="nested 2">
            <iframe id="frame" src="KogSem/CSkg1.pdf" width="100%" height="100%">
            </iframe>
        </div>
        <div id="nested 1"></div>
    </div>
</div>