# n8n Workflow: Update Zammad Roles by Excel

This repository contains an n8n workflow designed to update user roles in a Zammad instance based on an Excel file. It simplifies role management by automating the process and ensuring consistency.

## Features
- **Excel Integration**: Upload an Excel file with user emails and role IDs.
- **Automated Updates**: Automatically match users in Zammad by email and update their roles.
- **Error Tolerance**: Continue execution even if individual updates fail.
- **Configurable Inputs**:
  - `zammad_base_url`: Your Zammad instance URL.
  - `zammad_api_key`: Your Zammad API key.
  - `excel_source_url`: URL or path to the Excel file with user data.

## Setup
1. **Import the Workflow**:
   - Download the `.json` workflow file.
   - Import it into your n8n instance.
2. **Configure Variables**:
   - **`zammad_base_url`**: Set your Zammad instance's base URL.
   - **`zammad_api_key`**: Provide your Zammad API key.
   - **`excel_source_url`**: Provide the Excel file's URL containing user data.
3. **Run the Workflow**:
   - Execute the workflow to update roles based on the data in the Excel file.

## Contribution
We welcome contributions to improve this workflow. Please feel free to create an issue or submit a pull request.

---

**Note**: Ensure your Zammad API key has the necessary permissions to manage user roles.
