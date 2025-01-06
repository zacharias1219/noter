# **Full Stack Notes App - noter**

This project demonstrates the creation of **noter**, a full-stack web application inspired by Apple's Notes app. It leverages modern web development frameworks and technologies to provide a robust and responsive user experience.

---

## **Features**

- **User Authentication**:
  - Secure user registration and login using **JWT (JSON Web Tokens)**.
  - Password hashing for user data security.

- **Notes Management**:
  - Create, read, update, and delete notes.
  - Backend CRUD operations for persistent data storage.

- **Responsive UI**:
  - Built with **Nuxt.js** for a seamless and efficient user experience.
  - Styled using **TailwindCSS** for a clean, modern design.

- **Real-Time Feedback**:
  - Integrated frontend-backend connection for dynamic updates.

---

## **Tech Stack**

- **Frontend**: Nuxt.js with TailwindCSS
- **Backend**: Node.js with Prisma ORM and MySQL
- **Authentication**: JWT for session management
- **Database**: MySQL
- **Development Tools**:
  - MAMP for local database management
  - TablePlus for database visualization

---

## **Directory Structure**

```bash
├── app
│   ├── components
│   ├── pages
│   ├── styles
│   ├── services
├── prisma
│   └── schema.prisma
├── public
│   └── assets
├── constants
├── types
├── README.md
└── package.json
```

---

## **Setup and Installation**

### **Prerequisites**

1. **Node.js**: Version 16 or above.
2. **MySQL Database**: Install MAMP for local development.
3. **API Keys and Configuration**:
   - JWT secret key for authentication.

### **Steps**

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yourusername/noter.git
   cd noter
   ```

2. **Install Dependencies**:

   ```bash
   npm install
   ```

3. **Setup Environment Variables**:
   - Create a `.env.local` file in the root directory and include:

     ```env
     DATABASE_URL=mysql://root:password@localhost:3306/noter
     JWT_SECRET=your_jwt_secret_key
     ```

4. **Setup Prisma**:
   - Generate the Prisma client and apply migrations:

     ```bash
     npx prisma generate
     npx prisma migrate dev
     ```

5. **Run the Application**:

   ```bash
   npm run dev
   ```

   Access the app at `http://localhost:3000`.

---

## **How It Works**

### **Core Workflow**

1. **Authentication**:
   - User credentials are securely stored in MySQL with hashed passwords.
   - JWT ensures secure and scalable session management.

2. **Notes Operations**:
   - Users can create and manage notes with a user-friendly interface.
   - CRUD operations are implemented via API routes.

3. **Backend Database**:
   - Prisma ORM handles schema migrations and database interactions.
   - MySQL is used for reliable and fast data storage.

4. **Responsive Design**:
   - TailwindCSS ensures the app is visually appealing across devices.

---

## **Deployment**

1. **Build for Production**:

   ```bash
   npm run build
   ```

2. **Deploy**:
   - Use services like Vercel or AWS.
   - Configure `.env` for the production environment.

---

## **Future Enhancements**

- Add multi-user collaboration for shared notes.
- Implement note tagging and search functionality.
- Introduce dark mode for user preferences.

---

## **Contributing**

Contributions are welcome! Please fork the repository, create a feature branch, and submit a pull request.

---

## **License**

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---
