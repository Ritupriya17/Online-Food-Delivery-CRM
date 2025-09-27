# 🍽️ Online Food Delivery CRM

The **Online Food Delivery CRM** is a Salesforce-based application designed to streamline the end-to-end food delivery process for restaurants. It enables restaurant managers to manage menu items, process food orders, handle customer complaints, and generate insightful reports and dashboards — all within a single, integrated platform.

This capstone project was developed as a part of my **Salesforce Developer Virtual Internship** by **SmartBridge in Collaboration with Salesforce**, to demonstrate real-world CRM implementation in the food delivery domain.

---

## 🚀 Features

- **Restaurant & Menu Management**: Create and manage restaurant details and their menu items.  
- **Order Management**: Place, track, and manage food orders efficiently.  
- **Complaint Handling**: Log customer complaints and automatically update related order status.  
- **Role-Based Access**: Different access levels for Restaurant Managers, Delivery Agents, and Executives.  
- **Automated Notifications**: Email alerts for order confirmation and complaint resolution.  
- **Reports & Dashboards**: Monitor business performance, top-selling menu items, and complaints.  
- **Data Management**: Import/export data using Salesforce Data Import Wizard.  
- **Secure Access & Login**: Profile-based permissions, IP restrictions, and session settings.

---

## 🛠️ Tech Stack

- **Salesforce Platform** – Admin + Developer setup  
- **Lightning App** – Centralized app for managing restaurants, orders, and complaints  
- **Apex** – Classes for business logic:  
  - `FoodOrderService` – Recalculates totals and handles order logic  
  - `OrderLineItemHandler` – Syncs line item changes with parent orders  
  - `ComplaintHandler` – Updates food orders based on complaints  
- **Triggers** – Automated backend updates for Orders, Line Items, and Complaints  
- **SOQL / SOSL** – Data retrieval and search  
- **Salesforce Flows** – Automations for notifications and status updates  
- **Reports & Dashboards** – Visual analytics for performance and sales  
- **Field Level Security, Sharing Settings, Login IP Ranges** – Security controls

---

## 📑 Application Lifecycle

### 1. Restaurant & Menu Setup
**Restaurant Manager** adds restaurant records and creates menu items with details like name, category, and price. This acts as the foundation for placing orders.

---

### 2. Placing Food Orders
Orders are created by selecting menu items. Validation rules ensure required fields are filled. Total amounts are auto-calculated through Apex handlers and roll-up fields.

---

### 3. Order Line Items & Calculations
When items are added, updated, or deleted, the **OrderLineItemTrigger** calls the handler to recalculate the parent order total automatically.

---

### 4. Complaint Handling Workflow
Customers’ complaints are logged through the Complaint object. The **ComplaintHandler** updates the related order status (e.g., “Under Review” or “Resolved”) automatically using Apex logic.

---

### 5. Automated Notifications
Flows and Email Alerts send automatic emails:
- **Order Confirmation** – Sent to customers after order creation  
- **Complaint Resolution** – Sent when a complaint status is updated  

---

### 6. Reporting & Analytics
Built-in reports and dashboards provide:
- Top-selling menu items  
- Total revenue  
- Complaint statistics  
- Restaurant performance

Executives can analyze trends to make data-driven decisions.

---

### 7. Role-Based Access & Security
- **Restaurant Manager** – Full access to restaurants, orders, complaints  
- **Delivery Agent** – Restricted access (no sensitive fields like ID Proof)  
- **Executive** – Read-only access to reports and dashboards  
Security is enhanced using **Field Level Security**, **IP Ranges**, and **Session Settings**.

---

## 📊 Dashboards

- **Restaurant Business Overview** – Total orders, revenue, and top items  
- **Complaint Dashboard** – Complaint counts by type and resolution time  
- **Performance Dashboard** – Real-time restaurant metrics  

---

## 🚦 Installation & Setup

### 1. Clone Repository
```bash
git clone https://github.com/Ritupriya17/Online-Food-Delivery-CRM.git
cd Online-Food-Delivery-CRM
```

### 2. Deploy to Salesforce
- Use Salesforce Setup to create custom objects, fields, flows, triggers, and dashboards as described in documentation.
- Assign profiles, permission sets, and configure IP restrictions as needed.

### 3. Manual Setup
- Add sample Restaurant and Menu records.
- Create Food Orders and Complaint records for testing.
- Verify dashboards and reports.

---

## 🤝 Contributing

Contributions, bug reports, and suggestions are welcome!

- Fork the repository
- Open issues for bug reports or feature requests
- Create pull requests for proposed changes

---

## 👩‍💻 Author

Developed by Ritupriya17  
As part of a Salesforce Virtual Internship Capstone Project.
