# User Interface Specification Document

## Overview
This document describes the user interface (UI) specification for the User Management screen. It outlines the UI components, behavior, and requirements that developers need to implement. The goal is to provide a detailed guide to ensure consistency and usability in the UI design.

## UI Components

### 1. **Header Section**
   - **"New User" Button:**
     - **Functionality:** Opens a form to create a new user.
     - **Location:** Top-left corner of the user table.
     - **Appearance:** A blue button with the label "New User."
   - **"Hide Disabled User" Checkbox:**
     - **Functionality:** Toggles the visibility of disabled users in the user table.
     - **Location:** To the right of the "New User" button.
     - **Appearance:** A checkbox with the label "Hide Disabled User."

### 2. **User Table**
   - **Columns:**
     - **ID:** Unique identifier for each user (Integer).
     - **User Name:** Display name of the user (String).
     - **Email:** Email address of the user (String).
     - **Enabled:** Boolean value indicating if the user is active.
   - **Sorting:** Columns should be sortable by clicking on the column headers.
   - **Behavior:**
     - **Initial State:** By default, the table shows all users, sorted by ID.
     - **Actions:** Clicking on a row allows editing that user's information in the "New User" form.

### 3. **New User Form**
   - **Fields:**
     - **Username:** Text input for the user's username.
     - **Display Name:** Text input for the user's display name.
     - **Phone:** Text input for the user's phone number.
     - **Email:** Text input for the user's email address.
     - **User Roles:** Dropdown to select the user’s role(s) (e.g., Guest, Admin, SuperAdmin).
     - **Enabled:** Checkbox to enable or disable the user account.
   - **Validation:**
     - **Username, Display Name, and Email:** Required fields.
     - **Email:** Must be a valid email format.
   - **Behavior:**
     - **Save Button:** Clicking "Save User" will create or update the user based on the form's content.

### 4. **Save User Button**
   - **Functionality:** Commits the data entered in the "New User" form to the database.
   - **Location:** Top-right corner of the "New User" form.
   - **Appearance:** A blue button with the label "Save User."

## User Experience (UX) Guidelines
- **Feedback:** Provide real-time validation feedback as the user types in the form fields.
- **Error Handling:** Display clear error messages for any invalid input, such as "Email format is incorrect."
- **Confirmation:** After successfully saving a user, display a confirmation message, e.g., "User has been successfully saved."

