# Day_12
## Problem Statement
# StudentManagement Spring 1
## Problem Statement
Spring Flowers school wants to manage their students online:-
## User Stories :-
1. As a student. I should be able to see the Welcome page of my application.
2. As a Student. I should be able to see a MENU bar and School logo
3. As a Student. I should be able to see my information after clicking Student Profile Button
## Instructions:-
1. Please use HTML 5 and CSS 3 concepts
2. Try to make a proper application
3. Deploy the application on http server
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Spring Flowers School - Student Management</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f2f7f9;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #004080;
      color: #fff;
      display: flex;
      align-items: center;
      padding: 10px 20px;
    }
    header img.logo {
      height: 40px;
      margin-right: 15px;
    }
    header nav {
      flex-grow: 1;
    }
    header nav ul {
      list-style: none;
      display: flex;
      margin: 0;
      padding: 0;
    }
    header nav ul li {
      margin-right: 20px;
    }
    header nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    #welcome {
      text-align: center;
      padding: 40px 20px;
      font-size: 1.3em;
      color: #004080;
    }
    #welcome h1 {
      margin-bottom: 10px;
    }
    #profile-section {
      max-width: 600px;
      margin: 20px auto;
      background: white;
      border-radius: 8px;
      box-shadow: 0 0 10px #ccc;
      padding: 20px;
      display: none;
    }
    #profile-section img {
      height: 120px;
      float: left;
      border-radius: 50%;
      margin-right: 20px;
    }
    #profile-info {
      overflow: hidden;
    }
    #profile-info h2 {
      margin-top: 0;
      color: #004080;
    }
    button {
      background-color: #004080;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 4px;
      cursor: pointer;
      font-size: 1em;
      margin-top: 20px;
    }
    button:hover {
      background-color: #0066cc;
    }
    footer {
      text-align: center;
      padding: 10px;
      margin-top: 40px;
      color: #666;
    }
  </style>
</head>
<body>
  <header>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4a/School_icon.svg/2048px-School_icon.svg.png" alt="Spring Flowers School Logo" class="logo" />
    <nav>
      <ul>
        <li><a href="#" id="menu-home">Home</a></li>
        <li><a href="#" id="menu-profile">Student Profile</a></li>
      </ul>
    </nav>
  </header>

  <section id="welcome">
    <h1>Welcome to Spring Flowers School Student Management System</h1>
    <p>Manage your student profile and view school information online easily and securely.</p>
  </section>

  <section id="profile-section">
    <img src="https://example.com/student.jpg" alt="Student Image" />
    <div id="profile-info">
      <h2>Student Information</h2>
      <p><strong>Name:</strong> John Doe</p>
      <p><strong>Grade:</strong> 10</p>
      <p><strong>Roll Number:</strong> 23</p>
      <p><strong>Email:</strong> john.doe@example.com</p>
    </div>
  </section>

  <footer>
    &copy; Spring Flowers School
  </footer>

  <script>
    const profileSection = document.getElementById('profile-section');
    const welcomeSection = document.getElementById('welcome');
    const profileMenu = document.getElementById('menu-profile');
    const homeMenu = document.getElementById('menu-home');

    profileMenu.addEventListener('click', (e) => {
      e.preventDefault();
      welcomeSection.style.display = 'none';
      profileSection.style.display = 'block';
    });

    homeMenu.addEventListener('click', (e) => {
      e.preventDefault();
      profileSection.style.display = 'none';
      welcomeSection.style.display = 'block';
    });
  </script>
</body>
</html>
