# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨



**ANSWER**
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration Page</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: white;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1, h2 {
            text-align: center;
            color: #333;
        }
        ol {
            list-style-type: upper-roman;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 10px;
            text-align: left;
        }
        th {
            background-color: #333;
            color: white;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            font-weight: bold;
        }
        input, select {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        button {
            width: 100%;
            padding: 10px;
            background-color: #333;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #555;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome to Our Registration Page</h1>
        
        <h2>Ordered List (Roman Numerals)</h2>
        <ol>
            <li>Item One</li>
            <li>Item Two</li>
            <li>Item Three</li>
            <li>Item Four</li>
            <li>Item Five</li>
        </ol>
        
        <h2>External Image</h2>
        <img src="https://images.pexels.com/photos/30600496/pexels-photo-30600496/free-photo-of-vibrant-in-n-out-burger-exterior-in-los-angeles.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load" alt="Descriptive text" width="500">

        
        <h2>Contact List</h2>
        <table>
            <tr>
                <th>Name</th>
                <th>Address</th>
                <th>Mobile</th>
                <th>Email</th>
            </tr>
            <tr>
                <td>John Doe</td>
                <td>123 Main St</td>
                <td>+1234567890</td>
                <td>john@example.com</td>
            </tr>
            <tr>
                <td>Jane Smith</td>
                <td>456 Oak St</td>
                <td>+9876543210</td>
                <td>jane@example.com</td>
            </tr>
            <tr>
                <td>Robert Brown</td>
                <td>789 Pine St</td>
                <td>+1122334455</td>
                <td>robert@example.com</td>
            </tr>
            <tr>
                <td>Emily White</td>
                <td>101 Elm St</td>
                <td>+5566778899</td>
                <td>emily@example.com</td>
            </tr>
            <tr>
                <td>Michael Green</td>
                <td>202 Birch St</td>
                <td>+6677889900</td>
                <td>michael@example.com</td>
            </tr>
        </table>
        
        <h2>Registration Form</h2>
        <form>
            <div class="form-group">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your name" required>
            </div>
            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email" required>
            </div>
            <div class="form-group">
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" placeholder="Enter your password" required>
            </div>
            <div class="form-group">
                <label for="dob">Date of Birth:</label>
                <input type="date" id="dob" name="dob" required>
            </div>
            <div class="form-group">
                <label for="gender">Gender:</label>
                <select id="gender" name="gender">
                    <option value="male">Male</option>
                    <option value="female">Female</option>
                    <option value="other">Other</option>
                </select>
            </div>
            <div class="form-group">
                <label>Subscription:</label><br>
                <input type="checkbox" id="news" name="subscription" value="newsletter"> <label for="news">Subscribe to Newsletter</label>
            </div>
            <div class="form-group">
                <label>Membership Type:</label><br>
                <input type="radio" id="basic" name="membership" value="basic" required> <label for="basic">Basic</label>
                <input type="radio" id="premium" name="membership" value="premium" required> <label for="premium">Premium</label>
            </div>
            <button type="submit">Register</button>
        </form>
    </div>
</body>
</html>
