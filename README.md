/* Amazon-inspired Portfolio CSS for Jekyll */
/* main.css or portfolio.css */

:root {
  --primary-color: #232f3e;
  --secondary-color: #ff9900;
  --text-color: #333;
  --light-text: #666;
  --background: #f8f8f8;
  --card-bg: #fff;
  --border-color: #ddd;
  --highlight: #febd69;
  --success: #008577;
}

/* Base Jekyll styling */
.page-content {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
  color: var(--text-color);
  background-color: var(--background);
  padding: 20px;
}

.wrapper {
  max-width: 1200px;
  margin: 0 auto;
}

/* Typography */
h1, h2, h3, h4, h5, h6 {
  color: var(--primary-color);
  margin-bottom: 15px;
  font-weight: 600;
}

h1 {
  font-size: 2.5rem;
  border-bottom: 3px solid var(--secondary-color);
  padding-bottom: 10px;
  margin-bottom: 30px;
}

h2 {
  font-size: 2rem;
  margin-top: 40px;
  position: relative;
  padding-left: 15px;
}

h2::before {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 5px;
  background-color: var(--secondary-color);
  border-radius: 3px;
}

h3 {
  font-size: 1.5rem;
  margin-top: 25px;
  color: var(--secondary-color);
}

p {
  margin-bottom: 15px;
}

a {
  color: var(--secondary-color);
  text-decoration: none;
  transition: all 0.3s ease;
}

a:hover {
  color: var(--primary-color);
  text-decoration: underline;
}

/* Jekyll markdown content styling */
.markdown-content img {
  max-width: 100%;
  height: auto;
  display: block;
  margin: 20px 0;
}

/* Logo images */
.markdown-content img[alt="Amazon Logo"] {
  max-width: 150px;
  margin: 20px auto;
}

.markdown-content img[alt^="C"], 
.markdown-content img[alt="JavaScript"], 
.markdown-content img[alt="HTML"], 
.markdown-content img[alt="CSS"], 
.markdown-content img[alt="React"], 
.markdown-content img[alt="Node.js"], 
.markdown-content img[alt="MongoDB"], 
.markdown-content img[alt="MySQL"] {
  max-height: 50px;
  display: inline-block;
  margin-right: 15px;
  margin-top: 10px;
  margin-bottom: 25px;
}

/* Layout Elements */
.container {
  padding: 20px;
  background-color: var(--card-bg);
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
  margin-bottom: 30px;
}

hr {
  border: 0;
  height: 1px;
  background-color: var(--border-color);
  margin: 40px 0;
}

/* About Me Section */
.about-me {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  margin-bottom: 30px;
}

.fun-fact {
  background-color: var(--highlight);
  padding: 15px;
  border-radius: 8px;
  margin: 20px 0;
  font-style: italic;
  text-align: center;
}

/* Academic Details */
.academic-details ul {
  list-style-type: none;
  padding-left: 0;
}

.academic-details li {
  margin-bottom: 10px;
  position: relative;
  padding-left: 25px;
}

.academic-details li::before {
  content: '🎓';
  position: absolute;
  left: 0;
  top: 0;
}

/* Skills Section */
.skills-section {
  margin-bottom: 40px;
}

.skill-category {
  margin-bottom: 30px;
}

.skill-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 20px;
  margin-top: 15px;
}

.skill-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 15px;
  background-color: var(--card-bg);
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.skill-item:hover {
  transform: translateY(-5px);
}

/* Projects Section */
.project-card {
  background-color: var(--card-bg);
  border-radius: 8px;
  box-shadow: 0 3px 15px rgba(0, 0, 0, 0.1);
  padding: 25px;
  margin-bottom: 30px;
  transition: transform 0.3s ease;
}

.project-card:hover {
  transform: translateY(-5px);
}

.project-card h3 {
  color: var(--primary-color);
  border-bottom: 2px solid var(--secondary-color);
  padding-bottom: 10px;
  margin-bottom: 15px;
}

.stack, .features, .approach {
  margin-top: 15px;
}

.tag {
  display: inline-block;
  background-color: var(--highlight);
  color: var(--primary-color);
  padding: 5px 10px;
  border-radius: 20px;
  font-size: 0.85rem;
  margin-right: 8px;
  margin-bottom: 8px;
}

/* Amazon Domain Section */
.domain-section {
  background-color: var(--card-bg);
  border-radius: 8px;
  box-shadow: 0 3px 15px rgba(0, 0, 0, 0.1);
  padding: 25px;
  margin-bottom: 30px;
}

.service-card {
  background-color: var(--background);
  border-left: 4px solid var(--secondary-color);
  padding: 15px;
  margin-bottom: 20px;
  border-radius: 0 8px 8px 0;
}

/* Business Use Cases */
.use-case {
  background-color: var(--card-bg);
  border-radius: 8px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
  padding: 20px;
  margin-bottom: 25px;
  border-left: 5px solid var(--secondary-color);
}

.use-case h3 {
  margin-top: 0;
}

/* Contact section */
.contact-links {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin: 30px 0;
}

.contact-links a {
  display: inline-flex;
  align-items: center;
  padding: 10px 15px;
  background-color: var(--primary-color);
  color: white;
  border-radius: 5px;
  transition: all 0.3s ease;
}

.contact-links a:hover {
  background-color: var(--secondary-color);
  text-decoration: none;
}

/* Footer */
.site-footer {
  text-align: center;
  padding: 20px 0;
  margin-top: 50px;
  border-top: 1px solid var(--border-color);
  color: var(--light-text);
}

/* Responsive design */
@media (max-width: 768px) {
  .skill-grid {
    grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
  }
  
  h1 {
    font-size: 2rem;
  }
  
  h2 {
    font-size: 1.7rem;
  }
  
  h3 {
    font-size: 1.3rem;
  }
}

@media (max-width: 480px) {
  .skill-grid {
    grid-template-columns: 1fr;
  }
  
  .contact-links {
    flex-direction: column;
    align-items: center;
  }
  
  .page-content {
    padding: 10px;
  }
}
# Anjali Savalkar - Algorithmic Problem Solving Portfolio

## About Me
I'm Anjali Savalkar, a passionate web developer currently pursuing my degree in Computer Science at KLE Technological University. I enjoy transforming ideas into interactive and visually appealing websites. My interests lie in problem-solving, full-stack development, and applying technology to real-world problems.

### Fun Fact
**I love debugging code almost as much as building it—it’s like solving a mystery with logic!**

---

## Academic Details 🎓

- **Name**: Anjali Savalkar
- **SRN (Student Roll Number)**: 01FE22BCS196
- **Course Name**: Algorithmic Problem Solving
- **Course Code**: 24ECSE309
- **Course Instructor**: Prakash Hegade
- **University**: KLE Technological University
- **Portfolio Topic/Domain**: 
  ![Amazon Logo](https://upload.wikimedia.org/wikipedia/commons/a/a9/Amazon_logo.svg)

---

## Skills 💻

### Languages
- **C**  
  ![C](https://upload.wikimedia.org/wikipedia/commons/1/18/C_Programming_Language.svg)
  
- **C++**  
  ![C++](https://upload.wikimedia.org/wikipedia/commons/1/18/ISO_C%2B%2B_Logo.svg)
  
- **JavaScript**  
  ![JavaScript](https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png)

### Web Development
- **HTML**  
  ![HTML](https://upload.wikimedia.org/wikipedia/commons/6/61/HTML5_logo_and_wordmark.svg)
  
- **CSS**  
  ![CSS](https://upload.wikimedia.org/wikipedia/commons/d/d5/CSS3_logo_and_wordmark.svg)
  
- **React**  
  ![React](https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg)
  
- **Node.js**  
  ![Node.js](https://upload.wikimedia.org/wikipedia/commons/d/d9/Node.js_logo.svg)

### Databases
- **MongoDB**  
  ![MongoDB](images/mongo.png)
  
- **MySQL**  
  ![MySQL](images/mysql.png)

---

## Projects

### Netflix Clone
A replica of the popular Netflix homepage, featuring a clean, modern interface with responsive design. This project demonstrates my ability to work with HTML, CSS, JavaScript, and React to create a user-friendly streaming platform experience.

- **Stack**: React, CSS, JavaScript
- **Features**: Responsive Design, Carousel, Movie Grid

---

### Few-Shot Brain Tumor Segmentation
This project focuses on leveraging few-shot learning techniques for accurate segmentation of brain tumors. The goal was to use minimal labeled data while achieving high performance in detecting tumor regions in MRI scans.

- **Approach**: Few-Shot Learning, Transfer Learning, Semantic Segmentation
- **Dataset**: BraTS 2021
- **Model**: Custom CNN + Pre-trained Models (Unet)
- **Evaluation**: Mean Intersection over Union (mIoU), Dice Coefficient
- **Tools**: PyTorch, NumPy, OpenCV

---

### Shopper Commerce Website
A fully functional e-commerce website built with modern web technologies, offering a seamless shopping experience. Users can browse products, add to cart, and securely check out.

- **Stack**: HTML, CSS, JavaScript, React, Node.js, MongoDB
- **Features**: Product listing, cart system, order tracking, admin dashboard
- **Authentication**: User login, registration, and JWT-based session management

[View on GitHub](https://github.com/AnjaliSavalkar/stone-paper-scissors)

---

## Domain - Amazon

Amazon is a global technology company recognized for its innovation and leadership in multiple domains including e-commerce, cloud computing (AWS), digital streaming, and artificial intelligence. Its mission is to be "Earth's most customer-centric company," constantly striving to improve customer experience through technology and efficiency.

### Amazon Services:
#### Amazon Web Services (AWS)
The world's leading cloud computing platform, providing solutions for storage, computing, machine learning, security, and more.

#### E-commerce Platform
Offers a vast range of products through Amazon.com, with features like personalized recommendations, fast shipping, and customer reviews.

#### Prime Video & Digital Streaming
A popular streaming service offering movies, TV shows, and original content to millions of subscribers worldwide.

---

## Business Use Cases

### 1. Autonomous Delivery (Drones & Robots)
Amazon is developing advanced drone and robotics technologies to revolutionize last-mile delivery. Prime Air focuses on rapid package delivery via drones, while Scout uses autonomous ground robots.

**Goal:** Reduce delivery times, improve efficiency, and minimize the carbon footprint.

---

### 2. Satellite Internet (Project Kuiper)
Project Kuiper aims to provide high-speed, low-latency internet to underserved communities through a network of low Earth orbit (LEO) satellites.

**Goal:** Bridge the digital divide and bring internet access to billions globally.

---

### 3. Robotic Automation and AI for Supply Chain
Amazon is actively researching and developing intelligent warehouse robots and AI tools to optimize inventory management and demand forecasting.

**Goal:** Make the supply chain faster, smarter, and more efficient.

---

### 4. Quantum Computing (AWS Braket)
Through AWS Braket, Amazon is investing in quantum computing by giving developers and researchers access to quantum systems via the cloud.

**Goal:** Accelerate quantum research and make quantum computing more accessible.

---

### 5. Sustainable Packaging & Climate Pledge
Amazon is investing in machine learning to design right-sized, eco-friendly packaging and has launched the Climate Pledge to reach net-zero carbon by 2040.

**Goal:** Reduce environmental impact and lead in sustainable innovation.

---

### 6. AWS for Edge Computing
Amazon is investing heavily in edge computing through AWS, which brings computation and data storage closer to data sources like IoT devices. AWS's Greengrass extends AWS to local devices, enabling more efficient and faster decision-making.

**Goal:** To enhance real-time data processing for industries such as manufacturing, agriculture, and healthcare.

---

## Contact

You can reach me via:

- [GitHub](https://github.com/AnjaliSavalkar)
- [LinkedIn](https://www.linkedin.com/in/anjali-savalkar-39998925a)
- [Email](mailto:savalkaranjali6@gmail.com)

---

&copy; 2025 Anjali Savalkar. All rights reserved.
