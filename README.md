# **Creative Canvas** 🎨📄

Creative Canvas is a .NET Core application that empowers users to create profiles, share resumes, showcase projects, and collaborate seamlessly. Built with a focus on professional networking, the platform enhances user experience by enabling interactions through comments and easy-to-use profile management tools.

---

## **Features** 🚀

### **User Profiles**
- Create, view, and edit personalized profiles with profile pictures, banners, and a custom "About Me" section.
- Integrated resume management: Upload, update, and showcase resumes directly on profiles.

### **Resume Sharing**
- Securely upload resumes in PDF format with robust file validation.
- Replace or delete resumes seamlessly through an intuitive interface.

### **Project Portfolio**
- Showcase projects with titles, descriptions, and visibility settings (public or private).
- Upload project images and display project timelines, including start and completion dates.
- Enable collaboration through comment threads on each project.

### **Commenting System**
- Add and view comments on user profiles and projects to foster collaboration and feedback.

### **Authentication and Authorization**
- Secure login and registration with hashed passwords using **BCrypt**.
- Persistent authentication through cookie-based sessions.
- Role-based access ensures secure resource management.

### **Dashboard**
- Personalized user dashboard with quick access to profiles, resumes, and project settings.
- Manage account settings, including password updates and email changes.

---

## **Core Technologies** 🛠️

### **Backend**:
- **ASP.NET Core MVC**: Framework for structured and scalable application development.
- **Entity Framework Core**: ORM for seamless database interactions.
- **BCrypt**: Secure password hashing.

### **Database**:
- **SQLite Server**: Stores user data, resumes, projects, and comments.

### **Frontend**:
- **Razor Views**: Dynamic server-side rendering for a seamless user experience.

---

## **Entity Relationships** 🔗

- **User**:
  - One-to-one relationship with **Profile**.
  - One-to-many relationships with **Resumes** and **Projects**.
- **Profile**:
  - Includes user details, profile images, and banners.
  - Linked to comments for collaborative discussions.
- **Project**:
  - Includes titles, descriptions, images, and visibility settings.
  - Allows users to share and gather feedback through comments.
- **Comment**:
  - Associated with profiles or projects.
  - Authored by users to enhance collaboration.

---

## **Getting Started** 💻

Follow these steps to set up and run the project locally:

### **Prerequisites**
- Install [.NET SDK](https://dotnet.microsoft.com/download/dotnet/6.0)
- Install [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

### **Steps**
1. **Clone the Repository**:
   ```bash```
   ```git clone https://github.com/duttasah26/CreativeCanvas.git```
   ```cd CreativeCanvas```
2. **Restore Dependencies**:
	```dotnet restore```
3. **Apply Migrations and Update the Database**:
	```dotnet ef database update```
4. **Run the Application**:
	```dotnet run```
5. Access the Application: Open your browser and navigate to http://localhost:5000.



