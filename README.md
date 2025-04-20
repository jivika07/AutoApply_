# Job Matcher Application

A Next.js application that helps users match their skills with job opportunities.

## Features

- LinkedIn profile analysis
- Job matching based on skills
- Email/password authentication
- PDF resume parsing

## Getting Started

### Prerequisites

- Node.js 18+ and npm
- MongoDB (local or Atlas)

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

### Environment Setup

Create a `.env.local` file in the root directory with the following variables:

```
# NextAuth Configuration
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=jobmatcher-secret-key-2024

# MongoDB
MONGODB_URI=mongodb://localhost:27017/jobmatcher

# ProxyCurl API
PROXYCURL_API_KEY=7v9D-3nv0smq2ENLu0qfqw
```

#### Setting up MongoDB

1. Install MongoDB locally or use MongoDB Atlas
2. Update the `MONGODB_URI` in your `.env.local` file with your MongoDB connection string

### Running the Application

```bash
npm run dev
```

The application will be available at [http://localhost:3000](http://localhost:3000).

## Authentication

The application uses NextAuth.js with a credentials provider for authentication. Users can:

1. Register a new account at `/register`
2. Sign in with email and password at `/login`
3. Access protected routes when authenticated

## Troubleshooting

### Authentication Issues

If you're having trouble signing in:

1. Make sure your MongoDB connection is working
2. Check that the NextAuth secret is correctly set in the `.env.local` file
3. Ensure your application is running on the URL specified in `NEXTAUTH_URL`
4. Check the browser console and server logs for any error messages

### LinkedIn Profile Analysis Issues

If the LinkedIn profile analysis is not working:

1. Verify that the ProxyCurl API key is correct in the `.env.local` file
2. Ensure the LinkedIn URL is in the correct format (e.g., `linkedin.com/in/username`)
3. Check the browser console and server logs for any error messages

## License

This project is licensed under the MIT License.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
