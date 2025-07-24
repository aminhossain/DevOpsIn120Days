### **#120DaysOfDevOps | Day 4: CI/CD Pipelines & SDLC**

  

### **🚀 Today’s Mission:**
Understand **how code magically turns into apps** (without midnight server crashes!).

  

----------

**CI/CD Traditional Definition:**
CI/CD stands for **Continuous Integration** and **Continuous Delivery** (or **Continuous Deployment**), and it's a way to build, test, and deliver software faster and more reliably. In simple terms, CI/CD automates the process of putting new code into a live application. With **Continuous Integration**, developers frequently add (or "integrate") their code into a shared project. Each time code is added, it's automatically tested to make sure it doesn’t break anything. **Continuous Delivery** means that once the code passes all the tests, it’s ready to be released to users at any time - often with just one click. **Continuous Deployment** goes one step further and automatically releases the tested code to users without manual approval. The main goal of CI/CD is to deliver updates and new features quickly, with fewer bugs and less stress.

---

  

### **The Big Picture (With a Pizza Factory! )**

 
Imagine building a  **pizza delivery app**:

1.  **Chefs (Devs)**  write code (recipes).
    
2.  **Robots (CI/CD)**  test, build, and deploy (oven + delivery drones).
    
3.  **Customers (Users)**  get  **hot, fresh updates**—no waiting!

    

**This is CI/CD: Your code’s journey from laptop → cloud → user’s phone/computer.**

---

### **CI/CD --> Continuous Integration (CI) & Continuous Delivery (CD)**

#### **1. Continuous Integration (CI)**

-   **What?**  *"Merge code safely, 100x/day!"*
    
-   **How?**
    
    -   Code →  **GitHub**  →  **Automated Tests**  →  **Build**  →  Alert if broken.
        
-   **Real Example:**
    
    -   Netflix runs  **4,000+ tests**  per commit. No "works on my machine" excuses!
        

#### **2. Continuous Delivery (CD)**

-   **What?**  _"Always ready to deploy!"_
    
-   **How?**
    
    -   Build →  **Staging Environment**  →  **Manual ‘Go’ button**  → Production.
        
    **Note:**  CD =  **"Courier service for code"** - packaged and labeled, just needs delivery!
    

#### **3. Continuous Deployment (CD²)**

-   **What?**  _"Auto-ship every change!"_
    
-   **Who uses it?**
    
    -   Facebook, TikTok—**deploy 50+ times/day**.
        
    **DevOps Rule:**  If tests pass →  **auto-release**  (no humans slowing things).

---

### **Why CI/CD Awesome:**

-   **Faster updates**  (Netflix deploys  **1,000x/day!**).
    
-   **Fewer bugs**  (tests run  **before**  code goes live).
    
-   **Happy teams**  (no more 3 AM "fix the server!" calls).
-    **CI/CD = Safety Net**  → No more  _"It works on my laptop!"_  disasters.
    
-   **SDLC + DevOps**  → Faster releases, happier users,  **less burnout**.

   CI/CD = **Your code’s autopilot to users.**

---

### **Hands-On Tasks (30 mins Max)**

**1. Build a Mini CI/CD Pipeline**:

-   Use  **GitHub Actions**  to auto-run tests on a Python script.
    
**Code Example: (GitHub Action File - main.yaml)**

	name: CI  
	on: [push]  
	jobs:  
	  test:  
		runs-on: ubuntu-latest  
	    steps:  
	      - uses: actions/checkout@v4  
	      - run: python -m pytest  #Imagine you have a Python file for testing test.py!


**2. Spot the Bottleneck**:
     
   -   Find  **one inefficiency**  (e.g., "Why wait for all tests to finish?").

---

### **Interview Qs of the Day:**

1.  What’s the difference between Continuous Delivery and Deployment?
    
2.  How would you explain CI/CD to a 10-year-old?
    
3.  Why is monitoring part of the SDLC?
---

**DevOps Joke of the Day**: Without CI/CD, deploying code is like mailing a letter by  **pigeon**.

Cheers! 🚀 🚀🚀