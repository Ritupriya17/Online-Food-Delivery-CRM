# Online Food Delivery CRM 🍔
*A Salesforce-based CRM for managing food orders, deliveries, complaints, and dashboards.*

---

## 📌 Project Overview

The **Online Food Delivery CRM** is a comprehensive Customer Relationship Management system built on Salesforce, tailored for food delivery businesses. It automates and manages the entire food delivery process—from capturing customer orders, assigning delivery agents, tracking deliveries, handling complaints, sending notifications, and generating insightful dashboards.

This project was developed as a capstone for a Salesforce Virtual Internship.

---

## 🚀 Features

- **Order Management**: Seamless creation, tracking, and updating of customer orders.
- **Delivery Assignment & Tracking**: Automatic assignment of orders to available delivery agents and real-time tracking.
- **Complaint Handling**: Efficient logging, tracking, and resolution of customer complaints.
- **SMS Notifications**: Integration with Twilio for real-time SMS updates to customers and delivery agents.
- **Payment Gateway**: Mock integration for payment status and tracking.
- **Google Maps Visualization**: Route and delivery tracking using Google Maps Embed API.
- **Reporting & Dashboards**: Pre-built dashboards for sales trends, delivery performance, and customer satisfaction.

---

## 🛠️ Tech Stack

- **Salesforce Sales Cloud / Service Cloud**
- **Apex**: Backend logic, custom APIs, triggers, and classes.
- **Lightning Web Components (LWC)**: Modern Salesforce UI components.
- **Salesforce Flows**: Automation for business processes (order assignment, notifications, etc.).
- **Twilio API**: For sending SMS notifications.
- **Google Maps Embed**: For visualizing delivery routes.
- **Mock Payment Integration**: Simulated payment flows for demonstration.

---

## 📂 Repository Structure

```
/docs         # Project documents, screenshots, user guides
/src          # Salesforce metadata (Apex classes, LWC, Flows)
README.md     # Project overview and documentation
```

---

## 🎯 Use Cases

1. **Order Management**
   - Customers place orders via integrated interfaces.
   - Orders are logged in Salesforce for tracking and assignment.

2. **Delivery Assignment**
   - Orders are automatically assigned to available delivery agents based on location and workload.
   - Assignment logic implemented using Flows and Apex.

3. **Order Tracking**
   - Customers and agents can track delivery status in real-time.
   - Notifications are sent at key points (order confirmation, out for delivery, delivered).

4. **Complaint Handling**
   - Customers can raise complaints via web or phone.
   - Complaints are tracked, assigned to agents, and resolved with status updates.

5. **Reporting & Analytics**
   - Sales, delivery times, agent performance, and complaint types visualized in dashboards.
   - Reports can be filtered by date, agent, or region.

---

## 🔗 Integrations

- **Twilio SMS**
  - Sends SMS to customers when order status changes.
  - Notifies delivery agents of new assignments.

- **Google Maps Embed**
  - Visualizes delivery routes from restaurant to customer.
  - Displays estimated delivery time on dashboards.

- **(Mock) Payment Gateway**
  - Simulates payment status updates within the CRM.

---

## 📊 Dashboards

- **Sales Trends**: View sales over time, by day, week, or month.
- **Delivery Times**: Analyze average delivery durations and bottlenecks.
- **Agent Performance**: Compare delivery agents by volume and customer feedback.
- **Complaints by Type**: Track and categorize customer complaints for process improvement.

---

## 🚦 Installation & Setup

1. **Clone the Repo**
    ```bash
    git clone https://github.com/Ritupriya17/Online-Food-Delivery-CRM.git
    ```

2. **Deploy to Salesforce**
    - Use Salesforce CLI (sfdx) to deploy `/src` metadata to your Salesforce org.
    - Assign necessary permission sets and licenses.

3. **Configure Twilio**
    - Create a Twilio account.
    - Add Twilio credentials to Salesforce Custom Metadata/Settings.

4. **Google Maps API**
    - Obtain an API key for Google Maps Embed.
    - Configure the key in Salesforce Custom Metadata/Settings.

5. **Demo Data**
    - Import sample data files (if provided) from `/docs` for testing.


---

## 🤝 Contributing

Contributions, bug reports, and suggestions are welcome!
- Fork the repo and create a pull request.
- Open issues for bugs or feature requests.

---

## 👩‍💻 Author

Developed by **Ritupriya17**  
As part of a **Salesforce Virtual Internship Capstone Project**.

---

## 📄 License

This project is for educational/demo purposes. For commercial use, please contact the author.

---
