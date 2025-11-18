# Performance Testing of RESTful Booker API using Apache JMeter

## 📌 Project Overview
This project demonstrates API performance testing using **Apache JMeter** on the public REST API:

https://restful-booker.herokuapp.com/booking


The goal is to test the **GET /booking** endpoint under load and measure key performance metrics such as:
- Response Time (Avg, Min, Max)
- Throughput (Requests/sec)
- Error %
- Latency
- Success/Fail Ratio

This project is suitable for beginners learning **API Performance Testing**, **JMeter**, or preparing for interviews.

---

## 🧪 Test Plan Details
The JMeter Test Plan includes:

### **1️⃣ Thread Group**
- **Users (threads):** 50  
- **Ramp-up time:** 5 seconds  
- **Loop count:** 1  
- **Behaviour on error:** Continue  

### **2️⃣ HTTP Request**
- **Protocol:** https  
- **Domain:** restful-booker.herokuapp.com  
- **Path:** /booking  
- **Method:** GET  
- **Keep Alive:** Enabled  

### **3️⃣ Listeners**
- ✔ **View Results Tree** (for debugging responses)  
- ✔ **Summary Report** (to analyze performance metrics)

---

## 🚀 How to Run This Test

### **Steps:**
1. Install **Apache JMeter** (version 5.6.3 recommended).  
2. Download or clone this repository.  
3. Open the file:  


4. Before running → Save the test plan if JMeter prompts.  
5. Start with 1 Thread user (debug mode) and check:
- Response Code = 200  
- JSON response in View Results Tree  
6. Change threads to 50 and run a full load test.
7. Observe output in **Summary Report**.

---

## 📊 Example Metrics You Should Get
(Your results may vary depending on network conditions)

- **Average Response Time:** 100–300 ms  
- **Throughput:** 30–60 requests/min  
- **Error %:** 0%  
- **Max Response Time:** 500–1000 ms  

These values help identify:
- Server performance  
- Stability  
- Load behaviour  
- Response spikes  

---

## 📁 Files Included
| File | Description |
|------|------------|
| `Get_List_of_booking.jmx` | Main JMeter test plan |
| `summary.csv` | Optional exported report (if saved) |
| `README.md` | Project documentation |

---

## 🎯 Learning Outcomes
By using this project, you will understand:

- How to test a REST API with JMeter  
- How Thread Groups work  
- How to configure HTTP Requests  
- How to analyze performance metrics  
- How to interpret throughput & response time  
- How to handle errors and troubleshoot API tests  

---

## 👤 Author
**Uday Kumar Banda**  
GitHub: https://github.com/budaykumar  

---

## ⭐ Notes
- RESTful Booker API is a public test API, so response times may vary.  
- If you face SSL issues, change HTTP Request → `Implementation` to **HttpClient4**.  
- Use **View Results Tree** only for debugging (disable for real load tests to reduce overhead).  

---

