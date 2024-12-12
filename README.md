API Project Readme
Project Overview
This project is a Contact Management API that provides CRUD operations for managing contacts. It is built using .NET Core 6 and follows best practices for scalability, maintainability, and ease of use.
Features
•	Create Contacts: Add new contact entries.
•	Read Contacts: Fetch all or specific contact details.
•	Update Contacts: Modify existing contact details.
•	Delete Contacts: Remove contact entries.
•	Validation: Ensures all fields meet the specified validation rules.
•	Global Error Handling: Standardized error responses.
•	CORS Enabled: Allow cross-origin requests for local and public access.
Project Structure
API Project
│
├── Controllers
│   └── ContactController.cs
│
├── Models
│   └── Contact.cs
│
├── Services
│   └── ContactService.cs
│
├── Repositories
│   └── ContactRepository.cs
│
├── Middleware
│   └── ErrorHandlingMiddleware.cs
│
├── Data
│   └── ContactDbContext.cs
│
├── Program.cs
└── Startup.cs (if applicable)
Prerequisites
•	.NET Core 6 SDK


dotnet run
The API will be available at http://localhost:5239 by default.
API Endpoints
Base URL
http://localhost:5239/api/Contact
Endpoints
Method	Endpoint	Description
GET	/	Get all contacts
GET	/{id}	Get a contact by ID
POST	/	Create a new contact
PUT	/{id}	Update a contact by ID
DELETE	/{id}	Delete a contact by ID
Validation Rules
•	First Name: Required
•	Last Name: Required
•	Email: Must be a valid email address
CORS Configuration
Error Handling


