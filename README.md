---

# University Explorer

A simple web application that lets users search for universities by state in India. This project demonstrates how to connect **AWS Lambda**, **API Gateway**, and **S3 Static Website Hosting** to build a serverless web application.

---

## 🛠 Project Overview

The project consists of:

1. **Lambda Function (Backend brain 🧠)**

   * Holds a list of universities for each state.
   * Example: Searching for `"Telangana"` returns universities located in Telangana.

2. **API Gateway (Cashier 🧾)**

   * Provides a REST API interface for the Lambda function.
   * Whenever the API is called, it triggers the Lambda function.
   * Returns the list of universities as JSON data.

3. **Frontend Website (Shop counter 🖥)**

   * Built using **HTML**, **CSS**, and **JavaScript**.
   * Contains a search box where users type the state name.
   * Fetches data from the API Gateway URL and displays the results dynamically.

4. **S3 Hosting (Display counter 📦)**

   * Frontend files (index.html, style.css, script.js) are uploaded to an **S3 bucket**.
   * Bucket is configured for **Static Website Hosting**.
   * Provides a shareable URL for anyone to access the website.

---

## ⚡ How It Works

1. User opens the website.
2. User types a state name in the search box.
3. Frontend sends a request to the **API Gateway URL**.
4. API Gateway triggers the **Lambda function**.
5. Lambda returns the list of universities for that state.
6. Frontend displays the universities to the user.

**Flow:**

```
Frontend (Website) → API Gateway → Lambda → API Gateway → Frontend → User
```

---

## 📂 Project Structure

```
├── index.html       # Main webpage
├── style.css        # Styling for the webpage
├── script.js        # JS logic to fetch data from API
└── README.md        # Project documentation
```

---

## 🚀 Deployment

* **Lambda**: Create a function in AWS Lambda and write the backend logic.
* **API Gateway**: Link the Lambda function to a REST API and deploy.
* **S3 Hosting**: Upload frontend files to an S3 bucket and enable Static Website Hosting.

---

## 💡 Features

* Search universities by state.
* Serverless architecture using AWS.
* Easy to deploy and share via S3 URL.

---

If you want, I can also **rewrite this README in a shorter, super-clean GitHub style** that’s perfect for open-source projects. It will be easier to read and look professional on GitHub. Do you want me to do that?
