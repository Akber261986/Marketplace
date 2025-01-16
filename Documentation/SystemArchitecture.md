# System Architecture

## Overview
The system architecture outlines the components and their interactions within the marketplace project. It demonstrates how the frontend, backend, and third-party APIs work together to deliver functionality.

---

## Architecture Diagram
Below is a high-level outline of the architecture:

```
[Frontend (Next.js)]
      |
      |---[Sanity CMS API (Product, Order, Customer Queries)]
      |
      |---[Third-Party APIs]
             |---[Payment Gateway API]
             |---[Shipment Tracking API]
```

---

## Components

### **1. Frontend**
- Built with **Next.js 14** to ensure fast rendering and dynamic routing.
- Fetches data from Sanity CMS and interacts with third-party APIs as needed.

### **2. Backend (Sanity CMS)**
- **Database**:
  - Manages structured content like products, orders, and customer details.
  - Supports real-time updates to ensure the latest data is always available.
- **Custom Schemas**:
  - Defines models for products, orders, and customers.

### **3. Third-Party APIs**
- **Payment Gateway**:
  - Securely processes user transactions.
- **Shipment Tracking**:
  - Provides real-time updates on the status of orders.

---

## Workflow Examples

### **1. Product Browsing**
1. The user accesses the `/products` page on the frontend.
2. The frontend sends a GET request to the Sanity CMS API to fetch the product list.
3. The product data is dynamically rendered on the page.

### **2. Order Placement**
1. The user adds products to their cart and proceeds to checkout.
2. The frontend sends a POST request to the `/orders` API to save the order in Sanity CMS.
3. The payment gateway API processes the transaction.
4. Upon success, the order status is updated in Sanity CMS.

### **3. Shipment Tracking**
1. The user views their order details.
2. The frontend sends a GET request to the shipment tracking API using the order ID.
3. The shipment status and expected delivery date are displayed in real-time.

---

## Tools for Visualization
To create a visual diagram for this architecture, consider using:
- **Excalidraw**
- **Lucidchart**
- **Mermaid.js** (for Markdown support)

---

## Visual Diagram Example (Mermaid.js)
Here is an example of how you can represent the architecture in a Mermaid.js diagram:

```mermaid
graph TD
    A[Frontend (Next.js)] -->|Fetch Data| B[Sanity CMS API]
    A -->|Interact| C[Third-Party APIs]
    C --> D[Payment Gateway API]
    C --> E[Shipment Tracking API]
    B --> F[Products, Orders, Customers]
```

You can render this Markdown-supported diagram directly on platforms like GitHub that support Mermaid.js integration.
