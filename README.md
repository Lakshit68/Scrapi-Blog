# Blog Website

This project is a Strapi-based blog site configured to use a PostgreSQL database hosted on Render.

## Features
- Strapi CMS for content management
- PostgreSQL database (cloud-hosted on Render)
- Environment variables for secure configuration
- Ready for deployment and local development

## Getting Started

### 1. Clone the repository
```
git clone <your-repo-url>
cd Blog-website
```

### 2. Install dependencies
```
npm install
```

### 3. Configure environment variables
Edit the `.env` file with your database and secret values. Example:
```
DATABASE_HOST=dpg-xxxxxx.region.render.com
DATABASE_PORT=5432
DATABASE_NAME=your_db_name
DATABASE_USERNAME=your_db_user
DATABASE_PASSWORD=your_db_password
DATABASE_SSL=true
```

### 4. Start Strapi
```
npm run develop
```

Visit [http://localhost:1337/admin](http://localhost:1337/admin) to create your admin user and manage content.

## Content Types
- Posts (title, content, publishedAt, etc.)
- Authors (name, bio, etc.)

## API Permissions
To allow public access to your API endpoints:
1. Go to **Settings → Roles → Public** in the Strapi admin panel.
2. Enable the permissions you need (e.g., find, findOne for Posts).
3. Save changes.

## Troubleshooting
- If you see a 403 Forbidden error, check your API permissions.
- If you see a database connection error, verify your `.env` values and Render database status.

## Deployment
You can deploy this project to any platform that supports Node.js and can connect to your Render PostgreSQL database.

---

For more details, see the Strapi documentation: https://docs.strapi.io/
