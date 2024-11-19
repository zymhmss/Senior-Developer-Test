### **Duration**

- Maximum 24 hours.

### **Instructions**

1. **Project Setup and Submission**
    - Start with a fresh Laravel and React or Vue.js application.
    - Push the project to a **new public GitHub repository**.
    
    **( you can do separate projects for front-end and back-end if you want to and make sure to send two repos if they are in separate** 
    
    - Document the following in `README.md`:
        - Setup instructions (including migrations, seeders, and storage links).
        - How to run the project (frontend and backend commands).
        - API usage guide (if endpoints are implemented).
    - Share the **repository URL** upon completion.
    - Make **meaningful Git commits**:
        - Initial commit when starting.
        - Final commit upon completion.

---

### **Requirements**

### **1. Authentication & Authorization**

- Use **Laravel Breeze/Jetstream** with **React/Vue.js** integration.
- Implement **Role-Based Access Control (RBAC)**:
    - Roles: Admin, Manager, User.
    - Only Admins can manage users, companies, and employees.
- Seed initial users:
    - **Admin**: admin@admin.com / password
    - **Manager**: manager@company.com / password
    - **User**: user@company.com / password

### **2. CRUD Operations**

- Implement **CRUD** for the following models:
    1. **Companies**
        - Fields: Name, Email, Logo (image), Website.
    2. **Employees**
        - Fields: Name, Email, Phone, Profile Picture, Company (relation).
- Backend:
    - **Validation:** Use Form Requests.
    - **File Handling:** Store logos and profile pictures in `storage/app/public`.
        - Resize and validate images (e.g., using **Intervention/Image**).
- Frontend:
    - Create **dynamic forms** for adding/editing Companies and Employees.
    - Display data with **pagination**, **search**, and **filtering**.

### **3. Dashboard**

- **Admin Dashboard**:
    - Total Companies, Total Employees.
    - Recent Companies and Employees.
    - Role-based visibility (restricted access for non-admins).
- **Manager Dashboard**:
    - View assigned company’s employees only.
    - Statistics: Employee count, recent activities.
- Use **chart.js** or **echarts** for simple data visualization.

### **4. API Development**

- Develop **RESTful API Endpoints** for:
    - CRUD operations (Companies and Employees).
    - Secure API with **Laravel Sanctum/Passport**.
- API Documentation:
    - Use **Swagger/OpenAPI** or **Postman Collection** for documentation.

### **5. Frontend: React or Vue.js**

- **Dynamic Table Components**:
    - Implement sorting, searching, and filtering with paginated data.
- **State Management**:
    - Use **Vuex/Pinia** or **React Context/Redux**.
- **Reusable Components**:
    - Form fields (e.g., file upload with preview).
    - Modal dialogs for confirmations.

### **6. Testing**

- Backend:
    - **Unit and Feature Tests** for models, controllers, and API endpoints.
    - Test role-based access, validation failures, and CRUD operations.
- Frontend:
    - Write basic **unit tests** for components.
    - Use **Jest/Vitest**.

---

### **Bonus Features**

- **Push Notifications** using Laravel Echo & Pusher.
- **Real-time Updates** for the dashboard (e.g., recent companies/employees).
- **Role Management UI**: Allow admins to assign/revoke roles dynamically.
- **Dark Mode** toggle for the frontend.
- **Containerization** with **Docker** for easier setup.

---

### **Expected Skills**

- Proficiency in **Laravel**, **React/Vue.js**.
- Deep understanding of **RBAC**, **security best practices**, and **clean architecture**.
- Frontend **state management** and **component-based design**.
- Strong focus on **testing** and **documentation**.
- API development and real-time data handling.