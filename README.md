# 🛒 Local Mart

**Local Mart** is an online marketplace platform designed to connect local vendors with customers.  
It increases the visibility of local businesses by registering vendors on the website and listing their products online.  
Customers can conveniently browse a variety of local goods and support community businesses.

---

## ✨ Key Features

- ✅ **Vendor Registration** – Local vendors can easily create an account and start selling  
- ✅ **Vendor Login** – Secure login system for vendors to manage their profile and products  
- ✅ **Product Management** – Vendors can add products by linking image URLs and product details  
- ✅ **Product Browsing** – Customers can browse a diverse catalog of local products  
- ✅ **Separate Vendor & Product Pages** – Distinct pages for viewing vendors and their specific products  
- ✅ **Responsive Design** – Smooth experience across mobile, tablet, and desktop devices  
- ✅ **Data Persistence** – All vendor and product data stored securely

---

## 🛠️ Technologies Used

### Backend:
- 🟢 **Node.js** – JavaScript runtime for building scalable server-side applications  
- 🚂 **Express.js** – Web framework for Node.js to build APIs and server-side logic  
- 🍃 **MongoDB** – NoSQL database for storing vendor and product information  

### Frontend:
- 🧩 **HTML** – Markup language for creating the structure of web pages  
- 🎨 **CSS** – Stylesheets for designing beautiful and responsive layouts  
- ✨ **JavaScript** – For interactive and dynamic behavior in web pages  

### Containerization:
- 🐳 **Docker** – Platform to containerize the application for consistent deployment

### CI/CD:
- 🤖 **Jenkins** – Automate building, testing, and deploying the application

---

## 📦 Installation

1️⃣ **Clone the repository:**

    git clone https://github.com/YourUsername/Local-Mart.git

2️⃣ **Navigate to the project directory:**

    cd Local-Mart

3️⃣ **Install server-side dependencies:**

    npm install

4️⃣ **Start the backend server:**

    npm start

> The server will typically run on `http://localhost:3000` unless otherwise configured.

---

## 🤖 Jenkins for CI/CD

You can automate your build and deployment process using **Jenkins**.

### 📦 Set Up Jenkins Pipeline

1️⃣ **Install Jenkins and required plugins**  
Ensure Jenkins is installed on your machine, and you have the necessary plugins (e.g., Git, NodeJS, Docker).

2️⃣ **Set up a Jenkinsfile**  
In the root of your project, create a `Jenkinsfile` to define the CI/CD pipeline. Example:
```groovy
    pipeline {
        agent any
        stages {
            stage('Install Dependencies') {
                steps {
                    script {
                        sh 'npm install'
                    }
                }
            }
            stage('Run Tests') {
                steps {
                    script {
                        sh 'npm test'
                    }
                }
            }
            stage('Build and Deploy') {
                steps {
                    script {
                        sh 'npm run build'
                        sh 'npm run deploy'
                    }
                }
            }
        }
    }
```

3️⃣ **Run the Jenkins pipeline**  
After configuring your Jenkins pipeline, trigger the build process either manually or automatically on code changes.

4️⃣ **Monitor the build progress**  
Visit the Jenkins dashboard to monitor the build, test, and deployment status.

- 📚 [Jenkins Documentation](https://www.jenkins.io/doc/)

---

## 🐳 Docker Support

You can also run this project using **Docker**.

### 📦 Build and Run with Docker Compose

1️⃣ **Make sure Docker and Docker Compose are installed**  
2️⃣ **In the project root, run:**

    docker-compose up --build

3️⃣ **Visit the app in your browser:**

    http://localhost:3000

---

## 🚀 How to Use

### 🛒 **Vendor Features:**
- **Register** as a vendor by providing necessary details
- **Login** to manage products and view profile
- **Add Products** with title, description, price, and image URL

### 👥 **Customer Features:**
- **Browse Products** listed by different vendors
- **View Vendor Profiles** to see more products from the same vendor

> 💡 Simple and intuitive UI designed for ease of use on all devices.

---

