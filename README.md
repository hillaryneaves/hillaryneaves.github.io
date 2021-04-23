# hillaryneaves.github.io

<MIS 3033>
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
        body {
            font-family: Arial;
        }

        /* Style the tab */
        .tab {
            overflow: hidden;
            border: 1px solid #ccc;
            background-color: #f1f1f1;
        }

            /* Style the buttons inside the tab */
            .tab button {
                background-color: inherit;
                float: left;
                border: none;
                outline: none;
                cursor: pointer;
                padding: 14px 16px;
                transition: 0.3s;
                font-size: 17px;
            }

                /* Change background color of buttons on hover */
                .tab button:hover {
                    background-color: #ddd;
                }

                /* Create an active/current tablink class */
                .tab button.active {
                    background-color: #ccc;
                }

        /* Style the tab content */
        .tabcontent {
            display: none;
            padding: 6px 12px;
            border: 1px solid #ccc;
            border-top: none;
        }
    </style>
</head>
<body>

    <h2>Website for Hillary Neaves</h2>
    <p>Click on the tabs to learn more:</p>

    <div class="tab">
        <button class="tablinks" onclick="openCity(event, 'Home')">Home</button>
        <button class="tablinks" onclick="openCity(event, 'About')">About</button>
        <button class="tablinks" onclick="openCity(event, 'Projects')">Projects</button>
        <button class="tablinks" onclick="openCity(event, 'Skills')">Skills</button>
        <button class="tablinks" onclick="openCity(event, 'Employment History')">Employment History</button>
    </div>

    <div id="Home" class="tabcontent">
        <h3>Home</h3>
        <p>Hello</p>
    </div>

    <div id="About" class="tabcontent">
        <h3>About</h3>
        <p>Hello</p>
    </div>

    <div id="Projects" class="tabcontent">
        <h3>Projects</h3>
        <p>Hello</p>
    </div>

    <div id="Skills" class="tabcontent">
        <h3>Skills</h3>
        <p>Hello</p>
    </div>

    <div id="Employment History" class="tabcontent">
        <h3>Employment History</h3>
        <p>Hello</p>
    </div>

    <script>
        function openCity(evt, cityName) {
            var i, tabcontent, tablinks;
            tabcontent = document.getElementsByClassName("tabcontent");
            for (i = 0; i < tabcontent.length; i++) {
                tabcontent[i].style.display = "none";
            }
            tablinks = document.getElementsByClassName("tablinks");
            for (i = 0; i < tablinks.length; i++) {
                tablinks[i].className = tablinks[i].className.replace(" active", "");
            }
            document.getElementById(cityName).style.display = "block";
            evt.currentTarget.className += " active";
        }
    </script>

</body>
</html>
