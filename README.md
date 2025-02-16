# NYC Early Intervention – Service Coordinator Demo

## Overview

This application is a demo tool for NYC Early Intervention Service Coordinators. It allows service coordinators to manage child records, authorizations, and notes related to the services provided to children in the Early Intervention Program.

## Functionality and Features

### Login/Signup

*   **Service Coordinator Login:** Allows existing service coordinators to log in using their login name and password.
*   **Service Coordinator Sign Up:** Allows new service coordinators to create an account by providing their personal and contact information.

### Dashboard

*   **Welcome Message:** Displays a personalized welcome message with the service coordinator's first name.
*   **Logout Button:** Allows the service coordinator to log out of the application.

### Child Management

*   **Add Child:** Allows service coordinators to add new child records by providing the child's personal information, NYEIS ID, date of birth, referral date, initial IFSP date, and status.
*   **Edit Child:** Allows service coordinators to edit existing child records.
*   **Delete Child:** Allows service coordinators to delete child records (with confirmation).
*   **Children Table:** Displays a sortable table of child records, including their first name, last name, NYEIS ID, date of birth, referral date, initial IFSP date, and status.

### Contacts Management

*   **Add Contact:** Allows service coordinators to add new contact information for a child.
*   **Edit Contact:** Allows service coordinators to edit existing contact information for a child.
*   **Delete Contact:** Allows service coordinators to delete contact information for a child (with confirmation).
*   **Contacts Table:** Displays a sortable table of contacts for a selected child, including their name, phone number, address, email, and mobile phone.

### Authorizations Management

*   **Add Authorization:** Allows service coordinators to add new authorization records for a child, including the authorization ID, type, start date, end date, units approved, and status.
*   **Edit Authorization:** Allows service coordinators to edit existing authorization records for a child.
*   **Delete Authorization:** Allows service coordinators to delete authorization records for a child (with confirmation).
*   **Authorizations Table:** Displays a sortable table of authorizations for a selected child, including the authorization ID, type, start date, end date, units approved, status, units used, and units remaining.

### Notes Management

*   **Add Note:** Allows service coordinators to add new notes for a child, including the authorization, date, start time, end time, note content, category, QA category, and e-signature.
*   **Edit Note:** Allows service coordinators to edit existing notes for a child.
*   **Delete Note:** Allows service coordinators to delete notes for a child (with confirmation).
*   **Notes Table:** Displays a sortable table of notes for a selected child, including the authorization ID, date, start time, end time, note content, category, QA category, and e-signature.

## Data Storage

The application uses `localStorage` to store all data. This means that the data is stored locally in the user's browser and will be persisted across sessions.

## Reset Functionality

The application includes a "Reset" button that clears all data from `localStorage` and reloads the dummy data. This is a permanent action and will remove all user-created data.

## Technologies Used

*   HTML
*   CSS
*   JavaScript

## Code Structure

The code is structured into several functions that handle different aspects of the application's functionality. These functions include:

*   **Helper Functions:** Functions for formatting dates and times, calculating end times, and retrieving eligible authorizations.
*   **Storage Helpers:** Functions for getting, setting, and initializing data in `localStorage`.
*   **Delete Functions:** Functions for deleting records from `localStorage` (with confirmation).
*   **Sort Functions:** Functions for sorting data in the tables.
*   **Action Handlers:** Functions for handling actions selected from dropdown menus.
*   **Form Functions:** Functions for displaying and handling forms for adding and editing records.
*   **View Functions:** Functions for displaying the different views of the application.
*   **Login/Signup Functions:** Functions for handling user login and signup.
*   **Dashboard Functions:** Functions for displaying the dashboard and children table.
*   **Initialization:** The `initLocalStorage` function initializes the data in `localStorage` when the application is loaded.