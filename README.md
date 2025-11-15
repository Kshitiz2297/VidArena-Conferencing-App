🌐 VidArena: Full-Stack Video Conferencing Application

VidArena is a modern, responsive, and scalable video conferencing client built entirely with the Next.js App Router and professional-grade external services. It provides all the core functionalities of platforms like Zoom, including secure user authentication, instant meetings, and scheduled calls.

This project showcases expertise in building secure, highly performant full-stack applications using modern TypeScript and serverless architecture.

✨ Key Features

Secure Authentication: User login, sign-up, and profile management handled seamlessly by Clerk.

Real-Time Conferencing: Instant video/audio calls, screen sharing, and participant controls powered by the Stream Video SDK.

Meeting Management: Ability to start instant meetings, schedule future calls, and join meetings via invitation links.

Personal Room: Dedicated, permanent meeting room link for instant access.

Responsive UI: Fully responsive design using Tailwind CSS and shadcn/ui, ensuring a seamless experience on all devices (desktop, tablet, mobile).

Serverless Logic: Utilizes Next.js Server Actions for secure, efficient backend interactions without requiring a traditional REST API layer.

💻 Tech Stack Overview

This project is built using a modern stack designed for performance and scalability:

Frontend: Next.js 14 (App Router) is the core React framework for server-side rendering and routing.

Styling: Tailwind CSS provides a utility-first approach for rapid, responsive design.

Language: TypeScript is used throughout for type safety and cleaner, more scalable code.

Authentication: Clerk handles the full-stack user authentication and session management.

Video/WebRTC: The Stream Video SDK provides the reliable, real-time video and audio calling infrastructure.

UI Components: shadcn/ui is used for accessible, custom-styled interface elements (Dialogs, Buttons, etc.).

🚀 Getting Started (Local Development)

Follow these steps to get VidArena running on your local machine.

1. Prerequisites

Before starting, ensure you have the following accounts and software:

Node.js (LTS Version)

A Clerk Account (for authentication service keys)

A Stream Account (for video service keys)

2. Setup

Clone the Repository:

git clone [YOUR-REPOSITORY-URL]
cd VidArena-Video-App


Install Dependencies:

npm install
# or yarn install


3. Environment Variables (Critical)

You must configure your API keys to enable authentication and video features.

Create a file named .env.local in the root directory.

Populate it with your keys from Clerk and Stream:

# Next.js Public Base URL
NEXT_PUBLIC_BASE_URL=http://localhost:3000

# Clerk Authentication Keys 
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_...
CLERK_SECRET_KEY=sk_test_...

# Stream Video/Audio Keys
NEXT_PUBLIC_STREAM_API_KEY=your_stream_api_key
STREAM_SECRET_KEY=your_stream_secret_key


(Replace the placeholder values with your actual keys.)

4. Run the Application

Start the development server:

npm run dev


The application will be accessible at: http://localhost:3000
