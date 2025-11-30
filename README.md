# Blogging_Platform
A full-stack, responsive blogging platform that allows users to create, edit, and publish articles. It includes essential features like user authentication, an admin dashboard, editing, and comment functionality.
<hr>
## Features

- ✅ User authentication (registration, login)
- ✅ Blog creation, editing, and deletion
- ✅ Rich text editor with React Quill
- ✅ Comments and likes system
- ✅ Image upload with Cloudinary
- ✅ Responsive design with Tailwind CSS

- ### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local installation or MongoDB Atlas)

- Update the `.env` file with your configuration:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/blogging-platform
   JWT_SECRET=your_jwt_secret_key_here_change_in_production
   JWT_EXPIRE=7d

   # Cloudinary Configuration (for image uploads)
   CLOUDINARY_CLOUD_NAME=your_cloud_name
   CLOUDINARY_API_KEY=your_api_key
   CLOUDINARY_API_SECRET=your_api_secret
   ```
 Update the `.env` file:
   ```env
   REACT_APP_API_URL=http://localhost:5000/api
   ```

   The frontend will run on http://localhost:3000

## Usage

1. Register a new account or login with existing credentials
2. Create your first blog post using the rich text editor
3. Browse and search other blogs on the platform
4. Like and comment on blogs
5. View your profile and manage your blogs
6. Admin users can access the dashboard to view statistics

## Project Structure

```
blogging-platform/
├── backend/
│   ├── config/
│   │   ├── db.js
│   │   └── cloudinary.js
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── blogController.js
│   │   ├── commentController.js
│   │   └── adminController.js
│   ├── middleware/
│   │   ├── auth.js
│   │   └── upload.js
│   ├── models/
│   │   ├── User.js
│   │   ├── Blog.js
│   │   └── Comment.js
│   ├── routes/
│   │   ├── authRoutes.js
│   │   ├── blogRoutes.js
│   │   ├── commentRoutes.js
│   │   └── adminRoutes.js
│   ├── server.js
│   └── package.json
└── frontend/
    ├── public/
    ├── src/
    │   ├── components/
    │   │   ├── Navbar.js
    │   │   └── Footer.js
    │   ├── context/
    │   │   └── AuthContext.js
    │   ├── pages/
    │   │   ├── Home.js
    │   │   ├── Login.js
    │   │   ├── Register.js
    │   │   ├── CreateBlog.js
    │   │   ├── BlogDetail.js
    │   │   ├── Profile.js
    │   │   └── AdminDashboard.js
    │   ├── services/
    │   │   └── blogService.js
    │   ├── utils/
    │   │   └── api.js
    │   ├── App.js
    │   └── index.js
    └── package.json
```
## License

This project is licensed under the MIT License.
