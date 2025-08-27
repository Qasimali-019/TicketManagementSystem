# 🎫 Ticket Management System  

A **web-based Ticket Management System** built with **.NET 8, Blazor, and Razor Pages**.  
This system allows **users** to create and track support tickets, while **administrators** manage user accounts, ticket categories, priorities, and oversee workflows.  

---

## 🚀 Project Overview  
- **Users:** Can log in, create tickets, add attachments, and participate in discussions.  
- **Admins:** Can register users, assign tickets, update statuses, and manage categories/priorities.  
- **Database:** SQL Server (via Entity Framework Core).  
- **Authentication & Roles:** ASP.NET Core Identity.  

---

## 🛠️ Technologies Used  
- **.NET 8 (C#)**  
- **Blazor & Razor Pages**  
- **SQL Server**  
- **Entity Framework Core**  
- **ASP.NET Core Identity**  

---

## 🏗️ Architecture (Clean Architecture)  
- **Domain Layer:** Business models, DTOs, interfaces.  
- **Data Layer:** Repositories (`IGenericRepository<T>`, `ITicketRepository`, etc.), Unit of Work.  
- **Services:** Handle logic (`IAccountService`, `ITicketService`, etc.).  
- **Presentation Layer:** UI built with **Blazor** & **Razor Pages**.  

---

## 👥 User Roles  
- **Admin:**  
  - Register/manage users  
  - Manage tickets, categories, priorities  
- **User:**  
  - Create tickets  
  - Track status  
  - Join discussions  

---

## 🔄 Ticket Workflow  
1. **Admin** registers new users.  
2. **User** logs in and submits a ticket (attachments optional).  
3. **Admin** assigns ticket & updates status.  
4. **User & Admin** communicate through discussions.  
5. **Admin** closes/resolves ticket.  

---

## 📂 Project Structure  
TicketManagementSystem/
│── Domain/ # Entities, DTOs, Interfaces
│── Infrastructure/ # Data access, EF Core, Repositories
│── Application/ # Services, Business Logic
│── UI/ # Blazor & Razor Pages (Frontend)


## 🖼️ Screenshots 
<img width="889" height="481" alt="Screenshot 2025-08-19 191639" src="https://github.com/user-attachments/assets/ce89f109-9da4-4207-b8b4-d10de5596cd6" />



<img width="891" height="579" alt="Screenshot 2025-08-19 191652" src="https://github.com/user-attachments/assets/e2123029-ba0b-4681-b829-9935c0419b86" />
<img width="896" height="467" alt="Screenshot 2025-08-19 191705" src="https://github.com/user-attachments/assets/9957e87f-2552-4502-8097-44a74ba64ef4" />
<img width="894" height="557" alt="Screenshot 2025-08-19 191719" src="https://github.com/user-attachments/assets/1d4a7f8d-8bde-426e-8da7-215e0316b644" />
<img width="894" height="191" alt="Screenshot 2025-08-19 191751" src="https://github.com/user-attachments/assets/3154bf20-0595-4234-8ff4-03d7e2f78a3d" />
<img width="898" height="332" alt="Screenshot 2025-08-19 191802" src="https://github.com/user-attachments/assets/448aa51c-d8c2-410d-b835-8496a8d3a090" />
<img width="895" height="359" alt="Screenshot 2025-08-19 191810" src="https://github.com/user-attachments/assets/596d7418-79e2-48a1-9ad4-d9e1bc5636e8" />
<img width="882" height="453" alt="Screenshot 2025-08-19 191820" src="https://github.com/user-attachments/assets/f023eb64-a1e9-4dad-8b93-f485bab7bc9d" />
<img width="883" height="390" alt="Screenshot 2025-08-19 191834" src="https://github.com/user-attachments/assets/2d23d764-0206-4041-a96d-61a54c5595ec" />
<img width="885" height="365" alt="Screenshot 2025-08-19 191843" src="https://github.com/user-attachments/assets/645961a3-122a-400c-a122-f3c820f6dac5" />
<img width="886" height="478" alt="Screenshot 2025-08-19 191852" src="https://github.com/user-attachments/assets/c15bdd74-04b4-4f0c-829b-5c0dc7f3adf3" />
<img width="872" height="389" alt="Screenshot 2025-08-19 191901" src="https://github.com/user-attachments/assets/2410b2e6-8d08-49a0-99b2-8da4269b4cd7" />



## 1.  **Clone the repository**  
   git clone https://github.com/Qasimali-019/TicketManagementSystem.git
   cd TicketManagementSystem
Open in Visual Studio 2022

Open the solution file:

makefile
E:\TicketManagementUI\TicketManagementSystem.sln
Set up Database

Update connection string in appsettings.json to match your SQL Server.

dotnet ef database update
Run the project

Press F5 in Visual Studio OR

Run via CLI:
dotnet run
Login

Admin registers users.

Users log in to create and track tickets.

## 💡 Future Improvements
Add email notifications for ticket updates.

Enhance reporting/dashboard with charts.

Implement real-time updates via SignalR.

## 🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss.

## 📜 License
This project is licensed under the MIT License.
