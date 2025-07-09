# Saveetha_Admission_clone
## Date: 09.07.2025

## Objective:
To design a landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS. This activity reinforces skills in layout design, form creation, user input handling, responsive structure, and visual styling based on a real-world example.

## Tasks:
#### 1. Analyze the Landing Page Layout:
Observe the split-screen layout with a promotional section on the left and a form on the right.

Note the use of background images, text styling, and branding elements.

#### 2. Create the HTML Structure:
Use semantic tags like ```<section>, <header>, <form>, and <footer>``` to organize content.

Structure the form with input fields such as name, email, phone, password, city, state, course, specialization, captcha, and checkbox.

#### 3. Add Form Functionality:
Include appropriate input types (text, email, tel, password, select, etc.) with placeholders and labels.

Use the <button> element for the "APPLY NOW" action.

#### 4. Apply CSS Styling:
Implement a split layout using flexbox or grid.

Style the form elements with padding, shadows, background colors, and rounded borders.

Include hover effects and button transitions to match the original look.

#### 5. Incorporate Images and Branding:
Add the institution logo and use matching fonts and colors.

Place a background image or blurred overlay behind the form content if needed.

#### 6. Ensure Responsiveness:
Make sure the page adapts to different screen sizes using media queries.

Maintain readability and layout integrity on both desktop and mobile.

## HTML Code:
```
<!DOCTYPE html>
<html>
<head>
    <title>Saveetha Engineering College</title>
    <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>

    <div class="banner-image">
        <form class="enroll-form">
            <h2>Admissions Open 2025</h2>
            <br>
            <input type="text" placeholder="Enter Name *" required>
            <br><br>
            <input type="email" placeholder="Enter Email Address *" required>
            <br><br>
            <input type="tel" placeholder="Enter Mobile Number *" required>
            <br><br>
            <input type="password" placeholder="Any Password of Your Choice *" required>
            <br><br>

            <div class="input-row">
                <select required>
                    <option value="" disabled selected>State *</option>
                    <option>Andhra Pradesh</option>
                    <option>Arunachal Pradesh</option>
                    <option>Assam</option>
                    <option>Bihar</option>
                    <option>Chhattisgarh</option>
                    <option>Goa</option>
                    <option>Gujarat</option>
                    <option>Haryana</option>
                    <option>Himachal Pradesh</option>
                    <option>Jharkhand</option>
                    <option>Karnataka</option>
                    <option>Kerala</option>
                    <option>Madhya Pradesh</option>
                    <option>Maharashtra</option>
                    <option>Manipur</option>
                    <option>Meghalaya</option>
                    <option>Mizoram</option>
                    <option>Nagaland</option>
                    <option>Odisha</option>
                    <option>Punjab</option>
                    <option>Rajasthan</option>
                    <option>Sikkim</option>
                    <option>Tamil Nadu</option>
                    <option>Telangana</option>
                    <option>Tripura</option>
                    <option>Uttar Pradesh</option>
                    <option>Uttarakhand</option>
                    <option>West Bengal</option>
                    <option>Andaman and Nicobar Islands</option>
                    <option>Chandigarh</option>
                    <option>Dadra and Nagar Haveli and Daman and Diu</option>
                    <option>Delhi</option>
                    <option>Lakshadweep</option>
                    <option>Puducherry</option>
                    <option>Ladakh</option>
                    <option>Jammu and Kashmir</option>
                </select>

                <select required>
                    <option value="" disabled selected>City *</option>
                    
                </select>
            </div>
            <br>

            <div class="input-row">
                <select required>
                    <option value="" disabled selected>Course *</option>
                    <option>B.E B.tech</option>
                    <option>Lateral Entry</option>
                    <option>M.E</option>
                    <option>MBA</option>
                </select>

                <select required>
                    <option value="" disabled selected>Specialization *</option>
                    <option>CSE</option>
                    <option>IT</option>
                    <option>CS</option>
                    <option>AIML</option>
                    <option>AIDS</option>
                    <option>ECE</option>
                    <option>EEE</option>
                    <option></option>
                </select>
            </div>
            <br><br>

            <div class="policy-note">
                <input class="opt-check" type="checkbox" id="agree" name="agree" required>
                <label for="agree">
                    I authorize Saveetha Engineering College & its representatives to contact me with updates and notifications via Email/SMS/WhatsApp/Call. This will override DND/NDNC *
                </label>
            </div>
            <br><br>

            <button type="submit">APPLY NOW <span style="font-size:15px;">&#10095;</span></button>
            <br><br>
            <p>Already have an Account? <a href="index.html">Login</a></p>
            <br>
            <p>Resend Verification Email</p>
        </form>
    </div>

</body>
</html>
```
## CSS Code:
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body {
  height: 100%;
  width: 100%;
  font-family: Arial, sans-serif;
}

.banner-image {
  background-image: url("bg.jpg");
  background-size: cover;
  background-position: center left;
  background-repeat: no-repeat;
  min-height: 100vh;
  width: 100%;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  padding: 30px;
}

.enroll-form {
  width: 320px;
  padding: 16px;
  border-radius: 10px;
  background-color: rgba(0, 0, 0, 0.6);
  box-shadow: 0 0 15px rgba(255, 255, 255, 0.2), 0 0 10px rgba(255, 255, 255, 0.1);
  max-height: none;
  overflow: hidden;
}

input, select {
  width: 100%;
  padding: 6px;
  margin-bottom: 6px;
  border-radius: 5px;
  border: none;
  font-size: 13px;
}

input:focus, select:focus {
  outline: none;
  box-shadow: 0 0 4px #e28743;
}

.input-row {
  display: flex;
  justify-content: space-between;
  gap: 8px;
  margin-bottom: 6px;
}

.input-row select {
  width: 100%;
}

label, p, h2 {
  color: white;
  font-size: 12px;
}

h2 {
  text-align: center;
  margin-bottom: 10px;
  color: white;
  text-shadow: 0 0 5px #e28743;
}

.policy-note {
  display: flex;
  align-items: flex-start;
  gap: 6px;
  color: white;
  font-size: 12px;
  margin-bottom: 10px;
}

.opt-check {
  margin-top: 2px;
}

button {
  width: 100%;
  padding: 8px;
  background-color: #e28743;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-weight: bold;
  margin-top: 4px;
  transition: background-color 0.3s ease;
  font-size: 13px;
}

button:hover {
  background-color: #cf6f26;
}

p {
  text-align: center;
  margin: 6px 0;
}

a {
  color: white;
  text-decoration: underline;
}
```

## Output:
![image](https://github.com/user-attachments/assets/8ad39390-1d04-48b1-b960-65fa10eb3e04)

## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.
