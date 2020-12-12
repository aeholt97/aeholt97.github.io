<!doctype html>
<head>
    <link rel="stylesheet" href="read.css"/>
    <title>My Notes</title>
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
    <script>
      $(document).ready(function(){
        $("ul#pdfs a").click(function(e) {
            e.preventDefault();
            $("#frame").attr("src", $(this).attr("href"));
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
        <div id="nested">
            <ul id="pdfs">
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg1.pdf">kg1</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg2.pdf">kg2</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg3.pdf">kg3</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg4.pdf">kg4</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg5.pdf">kg5</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg6.pdf">kg6</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg7.pdf">kg7</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg8.pdf">kg8</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg9.pdf">kg9</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg11.pdf">kg11</a></li>
                <li><a href="https://aeholt97.github.io/KogSem/KG/CSkg12.pdf">kg12</a></li>
            </ul>
        </div>
        <div id="nested 2">
            <iframe id="frame" src="https://aeholt97.github.io/KogSem/KG/CSkg1.pdf" width="100%" height="100%">
            </iframe>
        </div>
        <div id="nested 1"></div>
    </div>
</div>