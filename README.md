# Medium-like Full-Stack Application

A lightweight blogging platform built as a fun experiment to explore serverless architecture using **Cloudflare Workers**. This project leverages modern technologies to create a seamless user experience with scalable and efficient backend services.

## 🛠 Features

- **User Authentication**: Secure signup and login using JWT.
- **Blog Management**: Create, read, update, and delete blog posts.
- **Input Validation**: Robust validation with Zod for reliable data handling.
- **Serverless Backend**: Powered by Hono on Cloudflare Workers for scalability.
- **Database Management**: Prisma ORM with PostgreSQL for efficient data handling.
- **Type Safety**: TypeScript across the entire stack for enhanced reliability.

## 🚀 Tech Stack

- **Frontend**: React, Tailwind CSS
- **Backend**: Hono Framework, Cloudflare Workers
- **Database**: PostgreSQL, Prisma ORM
- **Authentication**: JWT (JSON Web Tokens)
- **Validation**: Zod
- **Language**: TypeScript

## 🌟 Why It’s Cool

- **Serverless Architecture**: Utilizes Cloudflare Workers to eliminate the need for traditional server management, ensuring high performance and scalability.
- **Modern Stack**: Combines React with a serverless backend, offering a full-stack experience with cutting-edge technologies.
- **Efficient Development**: Shared types and validation logic using Zod streamline the development process and maintain consistency across frontend and backend.
- **Learning Experience**: Provides hands-on experience with serverless computing, API design, and modern full-stack development practices.

## 📦 Installation & Setup

### Prerequisites

- Node.js (v14 or later)
- npm or yarn
- PostgreSQL database

### Steps

1. **Clone the Repository**
    ```bash
    git clone https://github.com/yourusername/medium-like-app.git
    cd medium-like-app
    ```

2. **Setup Backend**

    ```bash
    cd backend
    npm install
    ```

    - **Configure Environment Variables**
      - Create a `.env` file in the `backend` directory:
        ```env
        DATABASE_URL="postgres://avnadmin:password@host/db"
        JWT_SECRET="your_jwt_secret"
        ```

    - **Initialize Prisma**
      ```bash
      npx prisma migrate dev --name init_schema
      npx prisma generate --no-engine
      ```

3. **Setup Frontend**

    ```bash
    cd ../frontend
    npm install
    ```

4. **Run the Application**

    - **Start Backend**
      ```bash
      cd backend
      npm run dev
      ```

    - **Start Frontend**
      ```bash
      cd ../frontend
      npm run dev
      ```

5. **Access the Application**
    - Open your browser and navigate to `http://localhost:3000` (or the port specified by your frontend setup).

## 📚 How to Use

1. **Sign Up**
    - Create a new account using the signup form.

2. **Login**
    - Authenticate using your registered credentials.

3. **Create Blog**
    - Navigate to the dashboard and create a new blog post.

4. **Manage Blogs**
    - View, edit, or delete your existing blog posts.

## 🔧 Future Improvements

- **Rich Text Editor**: Integrate a rich-text editor for enhanced blog post formatting.
- **User Roles**: Implement roles and permissions for different user types.
- **Comments & Likes**: Add commenting and liking features to increase user engagement.
- **Deployment**: Deploy the application to a live environment using platforms like Vercel or Netlify.
