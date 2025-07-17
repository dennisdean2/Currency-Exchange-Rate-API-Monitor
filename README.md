# Currency-Exchange-Rate-API-Monitor

## 📊 Project Overview

This project uses [Postman](https://www.postman.com/) to fetch and monitor live currency exchange rates via the [ExchangeRate-API](https://www.exchangerate-api.com/). It automatically checks for critical currency rates and verifies API health through scheduled monitoring.

As a beginner in APIs and integrations, this project simulates real-world API support tasks like:
- Monitoring endpoint health.
- Verifying key data values (currency rates).
- Documenting and debugging failures.

---

## 📈 API Used

- **Endpoint:**  
  `https://open.er-api.com/v6/latest/USD`

- **Method:**  
  `GET`

- **Response Example:**  
  Rates for currencies like EUR, GBP, JPY, and many others.

- **API Provider:**  
  [ExchangeRate-API](https://www.exchangerate-api.com/)

---

## 🛠️ Monitoring Setup (Postman)

- **Tool:** [Postman Monitors](https://learning.postman.com/docs/monitoring-your-api/setting-up-monitor/)
- **What It Does:**
  - Automatically calls the API at scheduled intervals.
  - Checks that key currencies exist (`EUR`, `GBP`, `JPY`).
  - Logs test pass/fail results.
  - Alerts (optional).

### ✔️ Example Tests:
- Confirm response status code is 200.
- Confirm `rates` object exists (defensive test to ensure data structure is present)
- Confirm essential currencies (`EUR`, `GBP`, `JPY`) are present.

---

## 📂 Project Files

- `/Currency_Exchange_Rate_API_Monitor.postman_collection.json`  
  Postman Collection file for API testing and monitoring.

- `/README.md`  
  This project documentation.

---

## 📊 Status and Goals

- Learned basics of API testing using Postman.
- Set up automated monitoring using Postman Monitors.
- Next Steps:
  - Expand tests to cover more currencies.
  - Add error logging and notifications.
  - Explore CI/CD integration for automated runs outside Postman.
