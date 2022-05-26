## User Management Page
<hr>

**Description:** A page is required to manage all the users' information and roles via a dynamic table and a submit form.
When the page is first loaded the administrator should see three main components on the page. These are the header, table and submit form.

**Details and functions of UI Components:**

- **Header:** contains three elements.
    - **1. Element:** Blue left-aligned "Create New User" button. If it is clicked it will clear the submit form and create an empty "New User" submit form. After filling it in you can add it to the table via clicking the "Save User Button" and then the submit form is also cleared. 
    - **2. Element:** Left-aligned "Hide Disabled Users" checkbox. It is located on the right side of the "Create New User" button.
    If it is checked it invokes an action which is hiding all the  users with "Enabled" status equals "false" in the table. If it is unchecked all the users are listed in the table.

    - **3. Element:** Blue right aligned "Save User" button. After filling in the submit form we click the "Save User" button to create a new user. After the creation of a new user the submit form will be cleared. The new user content will be added to the table. If the submit form is empty no post action is invoked. We will use the same button for the user update process. We select the row of the user from the table to get its content to the related input fields of the submit form. Then we update the required parts and save them via the "Save User" button. The selected row will be updated with the new information and the submit form will be cleared.

- **Body:** is equally split vertically into 2 sections (like columns) and contains 2 elements.
    - **1. Element:**  Dynamic table which is located in the first section of the body has the same width as the divided section and its height should be limited to display only 15 rows. The rest of the users could be displayed by scrolling down the scroll bar of the table if there are more than 15 users. The table consists of 4 columns with the headers ID, User Name, Email and Enabled. The headers' text alignment is left-aligned with a blue background color and every header has a sort button on its right side in the column which allows the administrator to list the users according to the specific header in ascending or descending order. The table's rows or columns are not editable, it is only allowed to select a row to transfer its content to the submit form to update it. If the content of the columns are overflowing then the overflowing part of the content should be displayed as three dots. The width of columns will be resizable so the user can change the width of the columns by dragging the borders and hereby overflowing contents of the column will be displayed clearly without three dots at the end. 
    - **2. Element:** Html submit form titled as "New User" which is located in the second section of the body so on the right side of the users table has the same width as the divided section and the same height as the users table. The submit form has 6 input fields and is split in two columns. The first column's width has the %25 width of the submit form to display the headings of input fields and the second column has %75 width of the submit form to display the input fields. The input fields are displayed in the following order with different validation rules.
        - Input field "Username" is a string data type so the type of the input field is set as "text" and the allowed max character number should be 50 (only letters allowed).
        - Input field "Display Name" has the type "text" and the allowed max character number should be 50 (only letters allowed).
        - Input field "Phone" should have the type "text" to store it in a better format like "+90-555-444-3322" (but only numbers allowed).
        - Input field "Email" should have the type "email" and the allowed max character number should be 50.
        - Input field "User Roles" should have the type "select" and it will be a dropdown select list to choose one of the user roles "Guest", "Admin" or "SuperAdmin"
        -Input field "Enabled" should have the type "checkbox" to set the actual status of the user. If checkbox is checked then the user is status "Enabled" will be set as "true", if not then the user status "Enabled" will be set as "false.
        - No input field can be left blank while posting the submit form via clicking the "Save User" button.



