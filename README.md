# n8n Workflow: Update Zammad Roles by Excel

This repository contains an n8n workflow designed to update user roles in a Zammad instance based on an Excel file. It simplifies role management by automating the process and ensuring consistency.

## Features
- **Excel Integration**: Upload an Excel file with user emails and role IDs.
- **Automated Updates**: Automatically match users in Zammad by email and update their roles.
- **Error Tolerance**: Continue execution even if individual updates fail.
- **Configurable Inputs**:
  - `zammad_base_url`: Your Zammad instance URL.
  - `excel_source_url`: URL or path to the Excel file with user data.

## Usage
1. **Import the Workflow**: Upload the provided `.json` file into your n8n instance.
2. **Set Variables**:
   - `zammad_base_url`: Your Zammad instance URL.
   - `excel_source_url`: URL of the Excel file containing user data.
3. **Authentication for Zammad**
- Create in the Node "Find Zammad User by email" and "Update User Roles" a Header Auth Authentication
- **Name**: Authorization
- **Value**: Bearer &lt;put here your zammad api token&gt;
4. **Run the Workflow**: Execute the workflow to update user roles based on the Excel data.

## Contribution
We welcome contributions to improve this workflow. Please feel free to create an issue or submit a pull request.

---

**Note**: Ensure your Zammad API key has the necessary permissions to manage user roles.
