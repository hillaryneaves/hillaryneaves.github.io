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
        
        #EmploymentHistory {
            background-color: floralwhite;
        }
        
        #Projects {
            background-color: floralwhite;
        }
        
        #Skills {
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
    </div>

    <div id="About" class="tabcontent">
        <h3>About</h3>
        <p>My name is Hillary Neaves and I am a junior at the University of Oklahoma. I am currently majoring in Management Information Systems with a minor in Marketing. I plan to graduate in May of 2022 with a Bachelors of Business Administration in MIS. While in college, I have served as the Chapter President of my sorority for two years, served on Crimson Wishes Executive Committee, and been part of the Management Information Systems Student Association. I have loved my time in college and I look forward to what is next!</p>
    </div>
    
    <div id="EmploymentHistory" class="tabcontent">
        <h3>Employment History</h3>
        <p>While in college, I have worked as a Receptionist at Rehabilitation Medicine of Oklahoma and have an upcoming Internship with American Fidelity as a Business Operations Intern. I am looking forward to my future Internship and I am thankful for all that I have learned as a Receptionist at RMO.</p>
    </div>

    <div id="Projects" class="tabcontent">
        <h3>Projects</h3>
        <p>One of the projects that I am most proud of is my Database project. The project took the entire semester and me and my team worked extremely hard on it. We created an ERD, used SQL to run predicitions, and used implementation to test our theories. The project taught me a lot of useful information that I still carry with me in my MIS courses and it taught me how to be a better team member. You can view my project <a href="https://drive.google.com/file/d/17wx1en2mBzfLpsdKhxEnldbcKe6cBhaF/view?usp=sharing" target="_blank">here.</a> </p>
    </div>

    <div id="Skills" class="tabcontent">
        <h3>Skills</h3>
        <p>
            Throughout my time in college, I have learned many different skills. These skills have 
            helped me to succeed in my courses and organizations, and I plan to utilize them in my 
            future career. The skills that I have gathered are:
                <ul>
                    <li>C#</li>
                    <li>Microsoft Office</li>
                    <li>Visual Studio</li>
                    <li>Databases</li>
                </ul>
        </p>
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
