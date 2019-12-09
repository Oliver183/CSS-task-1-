<!DOCTYPE html>

<html lang="en">

<head>
    <title>CSS Part 1</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles/main.css">
    <link rel="stylesheet" href="styles/csspart1.css">
    <link rel="stylesheet" href="https://code.jquery.com/qunit/qunit-2.9.2.css">
</head>

<body>
    <header>
        <nav id="navMain">
            <a href="index.html">Home</a> |
            <a href="wwwintro.html">WWW Intro</a> |
            <a href="htmlstructure.html">HTML Structure</a> |
            <a href="htmlcontent.html">HTML Content</a> |
            <a href="dataimport.html">Data Import Formats</a> |
            <a href="csspart1.html">CSS Part 1</a> |
            <a href="csspart2.html">CSS Part 2</a> |
            <a href="design.html">Design Issues</a>
        </nav>

    </header>
    <div id="divContent">
        <section id="sectionMain">
            <h1>CSS Part 1</h1>

            <section id="practicearea">
                <h2>Practice Area</h2>
                
            </section>
            
            <section id="studentcode">
                <h2>Student Code Area</h2>
                <style>
                    b {
                        color: #0000ff;
                        background-color: yellow;
                    }
                    p.cssArea1Class1{
                        text-align: center;
                        border-style: solid;
                        border-color:#0000ff;
                        border-width: 3px;
                        

                    }

                    #cssID {
                        color:#7f7f7f;
                        border-style: dashed;
                        border-color:#0000ff;
                        border-width: 3px; 

                    }

                    p.cssArea1Class2 {
                        background-color:rgba(0, 255, 0,.2)
                        
                    }
                    div ~ p {
                        font-weight: bold;
                        font-family: monospace;
                         
                    }

                    a:hover {
                        color: #ff0000; 
                        background-color: #ffff00;
                         font-family:serif;
                    }

                    #firstLine::first-line {
                        font-variant: small-caps;
                               }

                    #cssAttribute[target=_blank] {
                        font-size: 1.5em;

                    }

                    #namedColor {
                        color: tomato;

                    }

                    #hexColor {
                        color: #ff00ff ;

                    }

                    #rgbColor {
                        color: rgb(33,189,6);

                    }

                    #rgbaColor {
                        color: rgba(33,189,6,0.3);

                    }

                    #hslColor {
                        color: hsl(266,100%,50%);

                    }
                    #hslaColor {
                        color: hsla(266,100%,50%,0.3);

                    }

                    ol{
                        font-family: Verdana;
                        background-color: #669977;
                         Padding: 20px;
                    }

                    li{
                        margin-left:35px;
                        background-color: #a9e0a9;
                         Padding: 5px;
                    }

                    li.highlighted{
                        
                        background-color: black ;
                        color : white;
                    }

                    #bands{
                        font-family: sans-serif;
                        border-collapse: collapse;
                        width: 700px;
                    }

                     td{
                            border-width: 1px;
                            border:solid ;
                            border-color: #ddd;
                            Padding: 8px;
                            color: #669977;
                            border-width: 1px;
                    }

                    th {
                        
                        border: solid;
                        border-color: #ddd;
                        Padding: 8px;
                        padding-Top: 12px;
                        padding-Bottom: 12px;
                        text-align: Left;
                        background-color: #669977;
                        color: white;
                        border-width: 1px;
                    }

                    #bands tr:nth-child(even){background-color: #f2f2f2;}

                 </style>
                    <p class="studentP" > This paragraph contains text, <b > some of which is bold.</b > </p >
                    <section id="cssID" >
                    <p id="para001" class="cssArea1Class1" > This is a paragraph inside a section</p >
                    <p id="para002" class="cssArea1Class2" > This is <b > another</b > paragraph inside the same section</p >
                    <section class="cssArea1Class2" >
                    This is a section with the class cssArea1Class2.
                    </section >
                    </section >
                    <section id="cssMulitpleClass" >
                    <div id="divSibling" > A div with sibling paragraphs</div >
                    <p id="parra003" > A further paragraph</p >
                    <p id="parra004" > Yet another paragraph</p >
                    </section >
                    <section id="cssPseudo" >
                    <a href="#" id="pseudoClass" > Test link</a >
                    <p id="firstLine" > Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Metus dictum at tempor commodo ullamcorper a lacus. Aliquam ultrices sagittis orci a scelerisque purus semper eget. Ornare aenean euismod elementum nisi quis eleifend quam adipiscing vitae. Integer vitae justo eget magna fermentum iaculis eu non diam. </p >
                    </section >
                    <section id="cssAttributes" >
                    <a href="#" target="_blank" id="cssAttribute" > Another link</a >
                    </section >
                    <section id="colorExamples" >
                    <p id="namedColor" > This is colored using a HEX color value</p >
                    <p id="hexColor" > This is colored using a HEX color value</p >
                    <p id="rgbColor" > This is colored using a RGB color value</p >
                    <p id="rgbaColor" > This is colored using a RGBA color value</p >
                    <p id="hslColor" > This is colored using a HSL color value</p >
                    <p id="hslaColor" > This is colored using a HSLA color value</p >
                    </section >
                    <section id="cssList" >
                    <Ol id="cssOL" >
                    <li > Item One</li >
                    <li class="highlighted" > Item Two</li >
                    <li > Item Three</li >
                    <li > Item Four</li >
                    </Ol >
                    </section >
                    <section id="cssTable" >
                    <table id="bands" >
                    <tr >
                    <th > Genre</th >
                    <th > Band</th >
                    <th > Country</th >
                    </tr >
                    <tr >
                    <td > Rock</td >
                    <td > ACDC</td >
                    <td > Australia</td >
                    </tr >
                    <tr >
                    <td > Rythm and Blues</td >
                    <td > Jools Holland</td >
                    <td > UK</td >
                    </tr >
                    <tr >
                    <td > Jazz</td >
                    <td > Michael Bublé</td >
                    <td > Canada</td >
                    </tr >
                    <tr >
                    <td > POP</td >
                    <td > Lady Gaga</td >
                    <td > USA</td >
                    </tr >
                    <tr >
                    <td > Boogie Woogie</td >
                    <td > Axel Zwigenberger</td >
                    <td > Germany</td >
                    </tr >
                    <tr >
                    <td > Countrey and Western</td >
                    <td > Dollt Parton</td >
                    <td > USA</td >
                    </tr >
                    </table >
                    </section >

                    </section >
                    </section >
                    <aside id="asideMain" >
                    <div id="divAsideHeight" >
                    <h2 > Tips/Links</h2 >
                    <q class="tip" > Don't forget to backup you work on a regular basis.</q>
                    <q class="tip" > Don't forget to use the Browser Developer Tools to help debug your code.</q>
                    <q class="tip" > Don't forget to make sure your code is <a href="https://validator.w3.org/" target="_blank">validated</a></q>
                    <p > <a href="https://www.w3schools.com/html/html5_syntax.asp" target="blank" > W3Schools Coding Conventions</a > </p >
                    <p > <a href="https://loremipsum.io/generator/?n=2&t=p" target="_blank" > Lorem ipsum Generator</a > </p >
                    <p > <a href="https://validator.w3.org/#validate_by_input" target="_blank" > W3C Validator</a > </p >
                    </div >
                    </aside >
                    </div >

                    <footer id="footerMain" >
                    <nav id="navFooter" >
                    <a href="index.html" > Home</a > |
                    <a href="wwwintro.html" > WWW Intro</a > |
                    <a href="htmlstructure.html" > HTML Structure</a > |
                    <a href="htmlcontent.html" > HTML Content</a > |
                    <a href="dataimport.html" > Data Import Formats</a > |
                    <a href="csspart1.html" > CSS Part 1</a > |
                    <a href="csspart2.html" > CSS Part 2</a > |
                    <a href="design.html" > Design Issues</a >
                    </nav >
                    </footer >
                    <div id="qunit" > </div >
                    <div id="qunit-fixture" > </div >
                    <script src="https://code.jquery.com/qunit/qunit-2.9.2.js" > </script >
                    <script src="scripts/testCSS1.js" > </script >
                    </body >

                    </html >
