```markdown
# University Explorer

A simple web application to search for universities by state in India. This project demonstrates how to build a **serverless web application** using **AWS Lambda**, **API Gateway**, and **S3 Static Website Hosting**.

---

## 🛠 Project Overview

The project consists of:

1. **Lambda Function (Backend brain 🧠)**
   - Stores a list of universities for each state.
   - Example: Searching `"Telangana"` returns universities in Telangana.

2. **API Gateway (Cashier 🧾)**
   - Provides a REST API to access the Lambda function.
   - Triggers the Lambda whenever the API is called.
   - Returns university data in JSON format.

3. **Frontend Website (Shop counter 🖥)**
   - Built with **HTML**, **CSS**, and **JavaScript**.
   - Users can type a state in the search box.
   - Fetches data from the API Gateway and displays results dynamically.

4. **S3 Hosting (Display counter 📦)**
   - Frontend files (`index.html`, `style.css`, `script.js`) are uploaded to an **S3 bucket**.
   - Configured for **Static Website Hosting**.
   - Provides a public URL to access the website.

---

## ⚡ How It Works

1. User opens the website.
2. User enters a state name in the search box.
3. Frontend sends a request to the **API Gateway URL**.
4. API Gateway triggers the **Lambda function**.
5. Lambda returns the list of universities for the state.
6. Frontend displays the results to the user.

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

- **Lambda:** Create a function in AWS Lambda and write the backend logic.  
- **API Gateway:** Link the Lambda function to a REST API and deploy it.  
- **S3 Hosting:** Upload frontend files to an S3 bucket and enable Static Website Hosting.  

---

## 💡 Features

- Search universities by state.  
- Fully serverless architecture using AWS.  
- Easy deployment and shareable via S3 URL.  

---

You can add a **screenshot** of the website here to make the README more engaging.
```
