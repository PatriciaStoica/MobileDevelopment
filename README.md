Task Management Mobile App - Client Requirements


1. Project Idea
This application is designed to help users manage their daily tasks efficiently. Users can add tasks by entering a task description and setting a due date. Once tasks are added, they will be listed on the screen, where users can easily update or delete them. The goal is to provide a simple and intuitive interface that allows users to keep track of their to-dos and deadlines without technical complications.





2. Domain Details
The main entity in this application is the Task. Each task will have the following fields:

Task Description (string): A brief description of what the task entails.
Due Date (date): The deadline by which the task needs to be completed.
Task ID (integer): A unique identifier for each task (generated automatically).
Status (string): Indicates whether the task is "pending" or "completed."
Priority (string): An optional field where the user can mark the task as "low," "medium," or "high" priority.





3. CRUD Operations (3 points)
Each operation follows the Create, Read, Update, and Delete (CRUD) model. Here's how they function for the Task entity:

Create: 
Users will enter a task description and select a due date. Upon pressing the "Add" button, the task is created and added to the list. The app will validate that the fields are filled correctly before creating the task.

Read: 
All tasks will be displayed in a list format, showing the task description and due date. Users can view their entire task list and see what needs to be completed.

Update: 
Each task will have an "Edit" button next to it. When pressed, the user can modify the task description or due date, then save the changes. The task will update in real-time in the task list.

Delete: Users can remove any task from the list by pressing the "Delete" button. The task will be deleted immediately from the app.





4. Persistence Details

Local Database:
The app will store all CRUD operations (create, read, update, and delete) in the local database. This ensures that tasks are accessible even when the device is offline.

Server:
When the device is online, tasks will also be synced with the server. The server will persist:
	Create: New tasks added will be saved on the server.
	Update: Any changes to tasks will be synced with the server.
	Delete: When tasks are deleted, they will also be removed from the server.
	The local database acts as a backup, while the server ensures data is available across devices.




5. Offline Scenarios
When the device is offline, the app will continue to function as follows:

Create: 
Users can still add tasks, and these will be stored in the local database. Once the device comes back online, the app will sync the new tasks with the server.

Read: 
All tasks stored locally will be available for viewing, even when offline. The user can browse their tasks as usual.

Update: Users can edit tasks while offline, and the changes will be saved in the local database. When the device reconnects, the updates will be pushed to the server.

Delete: Users can delete tasks while offline. These deletions will be reflected locally, and when the app reconnects, the deletions will be synced with the server.




6. App Mockup 
