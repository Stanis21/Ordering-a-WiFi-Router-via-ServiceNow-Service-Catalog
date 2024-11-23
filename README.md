# Ordering a WiFi Router via ServiceNow Service Catalog  

## 🚀 Project Overview  
This project simplifies the process of ordering WiFi routers through the ServiceNow Service Catalog. It automates approval workflows, integrates email notifications, and provides secure, role-based access for a seamless IT equipment request experience.  

---

## 🌟 Features  
- **🖥 Self-Service Portal:** User-friendly interface for submitting router requests.  
- **🔄 Automated Workflows:** Approval and order fulfillment processes are automated.  
- **📋 Dynamic Input Fields:** Collects user inputs like router type, quantity, and delivery date.  
- **📧 Email Notifications:** Keeps users and managers informed at every step.  
- **🔐 Role-Based Access:** Ensures secure access based on user roles.  

---

## ⚙️ Setup Instructions  

### Prerequisites  
- ServiceNow Developer Instance ([Sign up here](https://developer.servicenow.com)).  
- Knowledge of Service Catalog, Workflows, and Email Notifications in ServiceNow.  

### Steps  
1. **Access ServiceNow Instance**  
   - Log in to your ServiceNow developer account.  
   - Request a personal developer instance.  

2. **Create a New Category**  
   - Navigate to `Maintain Categories`.  
   - Add a category like "IT Equipment Requests."  
   - Add relevant images or icons for better UX.  

3. **Add a Catalog Item**  
   - Navigate to `Maintain Items`.  
   - Create an item titled **"WiFi Router Request"** and assign it to the "IT Equipment Requests" category.  

4. **Define Variables**  
   - Add fields to capture inputs:  
     - Router Type (Dropdown).  
     - Quantity (Number).  
     - Delivery Date (Calendar).  
     - Additional Comments (Text area).  

5. **Design Workflow**  
   - Open the `Workflow Editor`.  
   - Create an approval workflow with stages:  
     - Request Submission → Manager Approval → Inventory Check → Order Processing.  

6. **Configure Notifications**  
   - Set up email templates for status updates at each step.  

7. **Test the System**  
   - Use impersonation to validate request submission, approval, and notifications.  

---

## 📋 Project Workflow  
1. **Request Submission**  
   - Users submit WiFi router requests via the Service Catalog.  
2. **Approval Process**  
   - Requests are routed to managers for approval.  
3. **Inventory Check**  
   - System verifies the availability of routers.  
4. **Order Processing**  
   - Approved requests trigger an order task.  
5. **Notifications**  
   - Email updates are sent to users and approvers.  

---

## 🛠 Technologies Used  
- **ServiceNow**: For catalog and workflow automation.  
- **Workflow Editor**: To design approval processes.  
- **Email Notifications**: To keep users informed.  

---

## ✅ Testing Scenarios  
- **Valid Requests:** Verify successful submission and approval workflows.  
- **Invalid Requests:** Check for appropriate error handling.  
- **High Volume:** Test system stability with multiple requests.  

---

## 🔧 Common Issues  
- **Missing Notifications:**  
  - Check email server configurations and triggers.  
- **Workflow Errors:**  
  - Debug transitions in the Workflow Editor.  
- **Access Problems:**  
  - Ensure roles and permissions are correctly set up.  

---

## 🚀 Future Enhancements  
- **Dynamic Catalogs:** Show relevant items based on user roles.  
- **Asset Integration:** Automatically update inventory after orders.  
- **Conditional Approvals:** Auto-approve low-cost items while routing high-cost ones for managerial approval.  

---

## 📜 License  
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.  

---

## 🤝 Contributing  
Contributions are welcome!  
1. Fork the repository.  
2. Create a feature branch (`git checkout -b feature-name`).  
3. Commit your changes (`git commit -m 'Add feature-name'`).  
4. Push to the branch (`git push origin feature-name`).  
5. Submit a pull request for review.  

---  

Feel free to customize the README to your needs. Let me know if you need further assistance!  
