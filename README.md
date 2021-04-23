# hillaryneaves.github.io

<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
        body {
            font-family: Arial;
            background-color: dimgray;
        }
        
        #Home {
            background-color: floralwhite;
        }
        
        #About {
            background-color: floralwhite;
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
        <p>Welcome to Hillary's personal website! I have used my knowledge of HTML, CSS, and JavaScript to create a website that showcases my projects, skills, employment history, and personal information. I hope that you enjoy! </p>
        <div style ="padding-left: 40%">
    <img src="https://media-exp1.licdn.com/dms/image/C4E03AQGWqdz6qJY2wg/profile-displayphoto-shrink_400_400/0/1587179768596?e=1624492800&v=beta&t=dMWyXxVMc5HxvaoXiSdqy0TS31n7K0jO_jfwC3jVvt4"/>
        </div>
    </div>

    <div id="About" class="tabcontent">
        <h3>About</h3>
        <p>My name is Hillary Neaves and I am a junior at the University of Oklahoma. I am currently majoring in Management Information Systems with a minor in Marketing. I plan to graduate in May of 2022 with a Bachelors of Business Administration in MIS. While in college, I have served as the Chapter President of my sorority for two years, served on Crimson Wishes Executive Committee, and been part of the Management Information Systems Student Association. I have loved my time in college and I look forward to what is next!</p>
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
