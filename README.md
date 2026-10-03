# 🚀 QuickBite - Online Food Delivery Web Application

**QuickBite** is a feature-rich, web-based food delivery platform connecting customers with local restaurants[cite: 21]. The platform allows users to browse menus, search and filter options, manage a cart, checkout securely, and track orders in real time[cite: 21].

This repository hosts the software testing deliverables, test case suites, bug reports, and final QA verification metrics for the platform.

---

## 📊 QA Testing Overview & Deliverables

Testing was conducted rigorously across customer-facing flows (desktop + mobile web) in a dedicated staging environment (`https://staging.quickbite-demo.app`)[cite: 15, 16].

* **Overall Requirements:** 18 documented requirements[cite: 18]
* **Total Test Scenarios:** 20 scenarios[cite: 18]
* **Total Test Cases:** 65 test cases (61 executed)[cite: 16]
* **Overall Test Coverage:** **93.8%**[cite: 14]
* **Test Pass Rate:** **70.5%**[cite: 14]
* **Total Defects Logged:** 18 defects (3 Critical, 6 High, 7 Medium, 2 Low)[cite: 1]

---

## 🛠️ Main Features in Scope

1. **Authentication & User Management:** Registration, secure Login, Logout, and Forgot/Reset Password[cite: 21].
2. **Restaurant Discovery:** Advanced search by name/cuisine and filtering/sorting by price, ratings, and delivery time[cite: 23].
3. **Menu & Cart Management:** Dynamic restaurant menus, opening/closing status, out-of-stock items, and single-restaurant cart logic[cite: 23, 24].
4. **Checkout & Payment:** Address management, minimum order value enforcement, card payment processing (via sandbox gateway), and Cash on Delivery[cite: 21, 24].
5. **Order Tracking & Notifications:** Live order tracking, order history, and push notifications / promotional preferences[cite: 21, 24, 25].
6. **Security & Responsive UI:** Basic black-box security (input sanitization, vulnerability checks) and responsive design across desktop, tablet, and mobile breakpoints[cite: 15, 21, 25].

---

## 📝 Bug Summary & Severity Distribution

| Severity | Count | % of Total |
| :--- | :--- | :--- |
| **Critical** | 3 | 16.7%[cite: 12] |
| **High** | 6 | 33.3%[cite: 12] |
| **Medium** | 7 | 38.9%[cite: 12] |
| **Low** | 2 | 11.1%[cite: 12] |

### 🔍 Key Open / Critical Findings:
* **BUG-002 (Critical):** No account lockout after repeated failed login attempts (Brute-force exposure)[cite: 3, 18].
* **BUG-011 (Critical):** Expired card is authorized by the sandbox payment gateway[cite: 8, 18].
* **BUG-017 (Critical):** SQL injection payload in login email field causes unhandled server error and exposes query info[cite: 11, 18].

---

## 📁 Repository Structure

```text
├── Test_Cases.pdf             # Document 1: Full suite of 65 test cases & requirements matrix[cite: 20]
├── Bug_Report.pdf             # Document 2: Detailed logs and reproduction steps for 18 defects[cite: 1]
├── QA_Final_Test_Report.pdf   # Document 3: Executive summary, coverage statistics, and release risks[cite: 14]
└── Test.jpg                   # Visual defect consolidation summary dashboard[cite: 19]
