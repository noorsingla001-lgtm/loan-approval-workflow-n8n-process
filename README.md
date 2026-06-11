# 🏦 Loan Approval Workflow Automation (n8n)

An automated loan approval and risk assessment pipeline built using **n8n**. This workflow processes incoming loan applications, categorizes them based on risk levels (Low, Medium, High), logs data into Google Sheets, and sends automated alerts accordingly.

---

## 🚀 Features

* **Automated Risk Assessment:** Dynamically categorizes loan applications based on financial and credit data.
* **Google Sheets Integration:** Automatically logs incoming data and status updates in real-time.
* **Multi-Tiered Alert System:** * 🟢 **Low Risk:** Streamlined processing and approval routing.
    * 🟡 **Medium Risk:** Triggers manual review alerts.
    * 🔴 **High Risk:** Instant high-priority alerts to mitigate risk.
* **Seamless Orchestration:** Fully visual and maintainable node-based architecture via n8n.

---

## 📸 Workflow Previews

### The n8n Blueprint
Here is the visual mapping of the automation workflow:
![n8n Project](./n8n%20project.png)

### Data Management
All application details are tracked and updated dynamically in a centralized spreadsheet:
![Google Sheet](./Google%20Sheet.png)

### Risk Alerts
Depending on the risk profile, the system triggers specific notifications:
* **High Risk Alert:** ![High Risk Alert](./High%20Risk%20Alert.jpeg)
* **Medium Risk Alert:** ![Medium Risk Alert](./Medium%20Risk%20Alert.jpeg)
* **Low Risk Status:** ![Low Risk](./Low%20Risk.jpeg)

---

## 🛠️ Tech Stack & Tools

* **Automation Engine:** [n8n](https://n8n.io/)
* **Database/Tracking:** Google Sheets
* **Communication/Alerts:** Email / Chat Webhooks (as configured in the workflow)

---

## ⚙️ Setup & Installation

To run this project locally or import it into your own n8n instance:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/noorsingla001-lgtm/loan-approval-workflow-n8n-process.git](https://github.com/noorsingla001-lgtm/loan-approval-workflow-n8n-process.git)
    ```
2.  **Import to n8n:**
    * Open your n8n instance.
    * Create a new workflow.
    * Click on the top-right menu and select **Import from File**.
    * Select the `loan automatation` JSON file from this repository.
3.  **Configure Credentials:**
    * Set up your **Google Sheets OAuth2** credentials within n8n.
    * Update the spreadsheet ID in the Google Sheet nodes to match your own sheet.
    * Configure your notification nodes (Email/Slack/Discord) with appropriate webhooks or API keys.
4.  **Activate:** Toggle the workflow to **Active** to start processing live loan applications.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
