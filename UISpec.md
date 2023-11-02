# User Interface Specification

_Version: 1.0_  
_Date: 2.11.2023_  
_Author(s): Emirhan Uysal_

---

## Table of Contents

1. Introduction
2. User Flow and Navigation
3. UI Component Specifications
4. Interaction Details
5. Standard Components and Styles
6. Version History

---

## 1. Introduction

- **Purpose**: This UI specification is done for P.I Works technical assignment.

---

## 2. User Flow and Navigation

## 2.1 Users Page

- **Landing**: User is greeted with a page where they can see a table of users registered to the system and option of creating new users to the system.

- **Table**: User shall be  able to see registered users in the system on a table. Following information should be avaliable for the user in the table,
    - ID
    - User Name
    - Email
    - Enabled

- **New User**: There should be a button which opens a form to create/ register a new user to the system.

- **Save User**: There should be a button to save a newly created user to the database. This button should be only active if all the required fields in the user creation form are filled.

- **Hide Disabled User**: There should be a radio button to hide disabled users from the table of users.

- **User Creation Form**: There should be a form where the required information are taken by user to create a new user.

## 2.2 Error Pages

- **Server Error Page**: There should be a page to notify that something has gone with the server/application side.

---

## 3. UI Component Specifications

### 3.1 User Page

- Header:
    - **New User**:
        - Purpose: To open "new user" form to create a new user.
        - Behavior: Clicking this button will activate the new user form.
        - Visual Properties: Text color: white, background color: blue, includes a plus sign and "New User" text inside.
    - **Hide Disabled User**:
        - Purpose: Hide the disabled users from the users table.
        - Behavior: Hide the disabled users from the users table when it is activated.
        - Visual Properties: Radio box with a label of "Hid Disabled User".
    - **Save User**:
        - Purpose: Save newly created user to the database.
        - Behavior: Using the information taken from the user creation from create/ register a new user in the database.
        - Visual Properties: Text Color: white, background color: blue, only active when all the required fields are filled in the form.

- Table:
    - All of the collumns should have a sorting option.
    - **ID**:
        - Purpose: Collumn represents the user's ID in the database.
        - Behavior: Display user's ID.
        - Visual Properties: Table collumn.
    - **User Name**:
        - Purpose: Collumn represents the user's User name.
        - Behavior: Display user's User name.
        - Visual Properties: Table collumn.
    - **Email**:
        - Purpose: Collumn represents the user's Email registered in the databse..
        - Behavior: Display user's Email.
        - Visual Properties: Table collumn.
    - **Enabled**:
        - Purpose: Collumn represents the user's enabled/disabled status.
        - Behavior: Display wheter user is enabled or not.
        - Visual Properties: Table collumn, display true if user is enabled false if disabled.

- Form:
    - **Title**:
        - Purpose: A title for the form.
        - Behavior: -
        - Visual Properties: Header tag that displays "New User".
    - **Username**:
        - Purpose: Input for user name.
        - Behavior: Takes the username from the user.
        - Visual Properties: Input tag for the username.
    - **Display Name**:
        - Purpose: Input for display name.
        - Behavior: Takes display name from the user as input.
        - Visual Properties: Input tag for the display name.
    - **Phone**:
        - Purpose: Input for phone number.
        - Behavior: Takes phone number from the user as input.
        - Visual Properties: Input tag for the phone number.
    - **Email**:
        - Purpose: Input for email.
        - Behavior: Takes email from the user as input.
        - Visual Properties: Input tag for the email.
    - **User Role**:
        - Purpose: Input for the user role.
        - Behavior: Gives three different roles for the user which are,
            - Guest
            - Admin
            - Super Admin 
        - Visual Properties: A dropdown menu containing the user roles.
    - **Enabled**:
        - Purpose: To enable/ disable a user.
        - Behavior: Checked if user is enabled, unchecked if user is disabled.
        - Visual Properties: A radio box.
---

## 4. Interaction Details

- 1. **New User Interaction**:
    - **Focus**: When the button is pressed its color should become darker indicating that it is being pressed.
    - **Click**: When the button is clicked it should make user creation form active.

- 2. **Hide Disable User Interaction**:
    - **Hover**: Hovering over the radio button should put it a glowing blue outline.
    - **Click**: Clicking the radio button should change its state from selected to deselected and vise verca.

- 3. **Save User Interaction**:
    - **Hover**: Hovering over the button should make its color darker.
    - **Click**: Clicking on the button should but an black outline around the button.
    - **Disabled State**: If any required information is missing on the user creation form, this button should be disabled. 

- 4. **User Form Interactions**:
    - 4.1 **Input Box**: 
        - **Selected**: When selected input box should have an glowing blue outline around it.
        - **Invalid**: When the save user button is clicked if the information in this input is invalid, it should have an red outline.
    - 4.2 **User Roler Dropdown**:
        - **Selection**: On selection a dropdown list of avalible options should be presented to user, user should be able to navigate through options by using arrow keys on the keyboard.
        - **Hover**: Hovered item on the dropdown should be highlighted with blue background.

---

## 5. Standard Components and Styles

## 5.1 Buttons

- **Primary Button**:
    - Color: Blue
    - Text color: White
    - Font: Arial
    - Hover Effect: Darkened background
    - Disabled State: Faded background color, no hover effect

## 5.2 Inputs

- **Line Input**:
    - Color: White
    - Text color: Black
    - Font: Arial
    - Hover Effect: Blue border
    - Selected Effect: Blue border

- **Dropdown**:
    - Color: White
    - Text color: Black
    - Font: Arial
    - Hover Effect: Change color to blue, text color to white

- **Radio Button**:
    - Selected: Blue check should be visinle inside a square.

## 5.3 Table

- **Table Header**:
    - Color: Blue
    - Text color: White
    - Font: Arial
    - Sorted Effect: Darkened background

- **Row**:
    - **Odd Row**:
        - Color: White,
        - Text color: Black,
        - Font: Arial
    - **Even Row**:
        - Color: Light Blue,
        - Text color: Black bold,
        - Font: Arial
---

## 6. Version History

| Version | Date       | Author        | Changes Made    |
|---------|------------|---------------|-----------------|
| 1.0     | 2.11.2023  | Emirhan Uysal | Initial Version |

---

