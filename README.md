# Ex09 Event Registration Web Application
## Date:06.10.2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:    
```
home page:

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Saveetha Engineering College</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background: linear-gradient(to right, #eef2f3, #f7f8f8);
      margin: 0;
      padding: 0;
    }

    .container {
      padding: 20px;
    }

    .logo {
      margin-top: 20px;
    }

    .college-logo img,
    .main-logo img {
      width: 200px;
      max-width: 80%;
      margin: 20px auto;
    }

    .register-button {
      background-color: #e0dcdc;
      color: red;
      padding: 15px 30px;
      font-size: 20px;
      font-weight: bold;
      border: none;
      margin: 30px auto;
      cursor: pointer;
      display: inline-block;
    }

    .runner-image {
      margin-top: 40px;
    }

    .runner-image img {
      width: 100%;
      max-width: 400px;
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Header Logo -->
    <div class="college-logo logo">
      <img src="college-logo.png" alt="Saveetha Engineering College Logo">
    </div>

    <!-- Main Emblem -->
    <div class="main-logo">
      <img src="emblem.png" alt="College Emblem">
    </div>

    <!-- Register Button -->
    <button class="register-button">REGISTER</button>

    <!-- Runner Image -->
    <div class="runner-image">
      <img src="runner-image.png" alt="Runner Graphic">
    </div>
  </div>
</body>
</html>

 events page:

 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sports Day Events</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background: url('sports-background.png') no-repeat center center;
      background-size: cover;
      color: #000;
      text-align: center;
    }

    .container {
      padding: 20px;
    }

    .college-logo img {
      width: 80%;
      max-width: 300px;
      margin-top: 20px;
    }

    h2 {
      color: darkblue;
      font-size: 28px;
      margin: 30px 0 20px;
    }

    .event-list {
      list-style-type: none;
      padding: 0;
      font-size: 24px;
      font-weight: bold;
    }

    .event-list li {
      margin: 15px 0;
    }

    .event-list li:nth-child(1) {
      color: red;
    }

    .event-list li:nth-child(2) {
      color: green;
    }

    .event-list li:nth-child(3) {
      color: orange;
    }

    .event-list li:nth-child(4) {
      color: purple;
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- College Logo -->
    <div class="college-logo">
      <img src="college-logo.png" alt="Saveetha Engineering College Logo">
    </div>

    <!-- Heading -->
    <h2>SPORTS DAY EVENTS</h2>

    <!-- Events List -->
    <ul class="event-list">
      <li>1. HOCKEY</li>
      <li>2. KABBADI</li>
      <li>3. FOOTBALL</li>
      <li>4. VOLLEYBALL</li>
    </ul>
  </div>
</body>
</html>

event registration form page:

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Event Registration Form</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background: url('form-background.png') no-repeat center center;
      background-size: cover;
      text-align: center;
    }

    .container {
      padding: 20px;
    }

    .college-logo img {
      width: 80%;
      max-width: 300px;
      margin-top: 20px;
    }

    h2 {
      color: darkred;
      font-size: 26px;
      margin: 30px 0 20px;
    }

    form {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    input[type="text"],
    input[type="number"] {
      width: 80%;
      max-width: 300px;
      padding: 12px;
      margin: 10px 0;
      border: none;
      background-color: #dcdcdc;
      font-size: 16px;
      text-align: center;
    }

    .form-label {
      font-size: 16px;
      font-weight: bold;
      color: #333;
      margin-top: 15px;
    }

    .register-btn {
      background-color: limegreen;
      color: black;
      font-size: 18px;
      font-weight: bold;
      border: none;
      padding: 14px 30px;
      margin-top: 20px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- College Logo -->
    <div class="college-logo">
      <img src="college-logo.png" alt="Saveetha Engineering College Logo">
    </div>

    <!-- Form Title -->
    <h2>EVENT REGISTRATION FORM</h2>

    <!-- Registration Form -->
    <form>
      <input type="text" placeholder="FIRST NAME" required>
      <input type="text" placeholder="LAST NAME" required>
      <input type="number" placeholder="AGE" required>
      <input type="text" placeholder="DEPARTMENT" required>
      <input type="text" placeholder="REGISTER NO" required>

      <input type="text" placeholder="EVENTS TO REGISTER:" required>

      <button type="submit" class="register-btn">REGISTER</button>
    </form>
  </div>
</body>
</html>

thankyou page:

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Thank You Poster</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      background: linear-gradient(to bottom, #dff3ff, #ffffff);
      text-align: center;
      color: #000;
    }

    .header {
      background: white;
      padding: 10px;
    }

    .header img {
      width: 300px;
    }

    .content {
      padding: 60px 20px;
    }

    h1 {
      font-weight: 800;
      font-size: 28px;
    }

    p {
      font-size: 22px;
      line-height: 1.5;
      margin-top: 40px;
    }

    .track {
      position: relative;
      height: 250px;
      background: linear-gradient(to bottom, #e0f2ff, #ffffff);
      overflow: hidden;
    }

    .track::before {
      content: "";
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url('https://i.imgur.com/TxvOlvK.png') no-repeat center/cover;
      /* Replace this with your own track image */
    }
  </style>
</head>
<body>

  <div class="header">
    <img src="https://upload.wikimedia.org/wikipedia/en/thumb/7/7b/Saveetha_Engineering_College_logo.png/220px-Saveetha_Engineering_College_logo.png" alt="Saveetha Engineering College Logo">
  </div>

  <div class="content">
    <h1>THANK YOU!</h1>
    <p>Thanks for participating and<br>
    stay tuned for further updates!<br>
    Hope you achieve more!</p>
  </div>

  <div class="track"></div>

</body>
</html>

```


## OUTPUT:
![alt text](<Screenshot (32).png>)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
