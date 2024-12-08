# Manage_Employee
How to Use Manage_Employee to Add, Edit, Delete, and Multi-Delete Employees
The Manage_Employee project allows users to manage employee records in a simple and efficient way. Below is a summary of the steps to Add, Edit, Delete, and Multi-Delete employees using the application.
1. Add Employee
To add a new employee:

Navigate to the Employee Management Section: Go to the section of the application where employees are listed.
Click the "Add Employee" Button: This will open a form where you can enter the employee's details, such as name, position, department, and salary.
Submit the Form: After filling in the required fields, click the Save or Submit button to add the new employee to the database.
2. Edit Employee
To edit an existing employee's details:

Navigate to the Employee List: Find the employee you wish to edit in the list.
Click the "Edit" Button: Each employee record will have an "Edit" button next to it.
Update the Details: The "Edit" button opens a form where you can modify the employee’s information, such as position, department, or salary.
Save the Changes: After making the necessary changes, click Save to update the employee record in the database.

3. Delete Employee
To delete a single employee:

Navigate to the Employee List: Find the employee you want to delete.
Click the "Delete" Button: There will be a "Delete" button next to each employee.
Confirm Deletion: A confirmation popup (using SweetAlert or a similar library) will appear, asking you to confirm the deletion.
Complete the Deletion: After confirming, the employee will be removed from the database.
4. Multi-Delete Employees
To delete multiple employees at once:

Select Employees: In the employee list, check the checkboxes next to the employees you wish to delete.
Click the "Delete Selected" Button: This button will trigger a confirmation popup asking if you are sure about deleting the selected employees.
Confirm Deletion: If confirmed, the selected employees will be deleted in one batch. This can be done via a POST request to the server, which processes the deletion of all selected employee records.
Final Confirmation: Once the deletion is successful, a success message will appear, and the page will reload to reflect the changes.
Implementation Details
Add/ Edit: Handled by HTTP POST requests in the controller, where the employee data is passed and saved/updated in the database.
Delete: Performed through a button click, triggering a confirmation popup (using libraries like SweetAlert2), and if confirmed, a DELETE request is made to the backend to remove the employee.
Multi-Delete: Similar to the single delete, but multiple employees can be selected using checkboxes. After selecting, the deletion happens via a POST request with an array of employee IDs.

![image](https://github.com/user-attachments/assets/072774ae-af1f-40a6-a6b3-72185c9091da)

![image](https://github.com/user-attachments/assets/6887c60e-f37f-455f-b5ac-9589e98bec0c)

![image](https://github.com/user-attachments/assets/f3616fc6-ed0f-4f95-b42c-f050423dc8ea)

![image](https://github.com/user-attachments/assets/ef00b622-d87b-4575-b90c-67180aeeef25)



