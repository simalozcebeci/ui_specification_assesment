## User Management Screen Specification Document

### Overview
This document outlines the requirements and behavior of the user management screen.
It provides detailed information on the UI components, their functionality, and expected interactions. 
The goal is to help developers create a user-friendly interface for managing users within an application, allowing administrators to view, create, edit, and disable users.

### Requirements
1. **View Users**: Display a list of existing users.
2. **Add New User**: Provide a form for creating new users.
3. **Edit User**: Allow modifications to existing users.
4. **Enable/Disable User**: Enable or disable users.
5. **Role Assignment**: Assign roles to users.

### Initial View
When the user management screen is first loaded, you should see:
- A table listing existing users.
- A "New User" button.
- A checkbox to hide/show disabled users.
- An empty form for adding or editing users.

### UI Components and Behavior

#### 1. User Table
- **Columns**: 
  - ID
  - User Name
  - Email
  - Enabled
- **Sorting**: Each column should be sortable.
- **Rows**: Each row represents a user with their ID, username, email, and enabled status.
- **Actions**: Clicking on a row should fill the "New User" form with the selected user's details for editing.

#### 2. New User Button
- **Location**: Top left of the screen.
- **Functionality**: Opens the "New User" form for creating a new user.
- **Behavior**: Clears any data in the form and resets it for new user input.

#### 3. Hide Disabled Users Checkbox
- **Location**: Next to the "New User" button.
- **Functionality**: When checked, hides disabled users from the user table.
- **Behavior**: Filters the user table to show only enabled users.

#### 4. New User Form
- **Fields**:
  - Username: Text input.
  - Display Name: Text input.
  - Phone: Text input.
  - Email: Text input.
  - User Roles: Dropdown menu (options: Guest, Admin, SuperAdmin).
  - Enabled: Checkbox.
- **Buttons**:
  - Save User: Saves the user details (for both creating and editing users).
- **Behavior**:
  - **Creating a New User**: Fill in the fields and click "Save User" to create a new user.
  - **Editing an Existing User**: Populate fields with the selected user's details, modify as needed, and click "Save User" to update the user.

### Example User Interaction

1. **Viewing Users**:
   - By default, the user table shows all users.
   - Check the "Hide Disabled User" checkbox to filter out disabled users.

2. **Adding a New User**:
   - Click the "New User" button.
   - Fill out the form with the new user's details.
   - Select appropriate roles from the "User Roles" dropdown.
   - Check or uncheck the "Enabled" checkbox based on the user status.
   - Click "Save User" to add the new user to the table.

3. **Editing an Existing User**:
   - Click on a user row in the table.
   - Modify the user details in the form.
   - Click "Save User" to update the user information.

4. **Enabling/Disabling a User**:
   - Edit the user and check/uncheck the "Enabled" checkbox.
   - Click "Save User" to apply the changes.

