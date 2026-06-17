# Enterprise HRMS Next.js Setup

## Deployment Instructions

### Option 1: Quick Deployment to Vercel
1. Unzip this folder.
2. Push the files to a new GitHub repository.
3. Import the repository into **Vercel**.
4. In Vercel, add an Environment Variable named `DATABASE_URL` containing your live PostgreSQL connection string (from Supabase, Neon, etc.).
5. Click **Deploy**. Vercel will automatically handle dependencies, build steps, database schemas, and your dynamic production server.

### Option 2: Local Verification
1. Run `npm install`
2. Rename `.env.example` to `.env` and fill in your database credentials.
3. Run `npx prisma db push` to generate database schemas.
4. Run `npm run dev` to launch the local web server.
