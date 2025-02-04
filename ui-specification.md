# User Management Screen - UI Specification

## 1. Overview
This document provides the specifications for the User Management screen, describing UI components, expected behavior, and user interactions.

## 2. Requirements
- Display a list of users with ID, Username, Email, and Enabled status.
- Allow adding new users with Username, Display Name, Phone, Email, User Roles, and Enabled status.
- Enable user filtering and sorting options.
- Support saving user information.

## 3. UI Components

### **User List Table**
| Column       | Description                          |
|-------------|--------------------------------------|
| ID          | Unique identifier for the user.     |
| User Name   | The username of the account.        |
| Email       | Email address of the user.          |
| Enabled     | Boolean status (true/false).        |

- Sorting and filtering should be available for each column.
- "Hide Disabled User" checkbox should filter out disabled users.

### **New User Form**
| Field        | Type    | Description |
|-------------|--------|-------------|
| Username    | Text   | Required, unique. |
| Display Name | Text   | Optional. |
| Phone       | Text   | Optional. |
| Email       | Email  | Required, unique. |
| User Roles  | Dropdown | Multiple selection (Guest, Admin, SuperAdmin). |
| Enabled     | Checkbox | Default: unchecked. |

### **Buttons**
- **+ New User**: Opens the "New User" form.
- **Save User**: Saves user data and updates the list.

## 4. Behavior
- When clicking "+ New User", the form should clear existing data.
- "Save User" validates required fields before saving.
- If a user is successfully saved, a confirmation message appears.

## 5. Initial View
- The user list table is displayed with existing users.
- The "New User" form is empty by default.
