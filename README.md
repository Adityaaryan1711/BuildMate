# BuildMate

An AI-powered project builder that helps you generate and manage projects with intelligent suggestions. BuildMate leverages cutting-edge AI technology to streamline project creation and provide smart recommendations for your development needs.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Folder Structure](#folder-structure)
- [Environment Variables](#environment-variables)
- [Installation](#installation)
- [How to Run Locally](#how-to-run-locally)
- [Deployment with Vercel](#deployment-with-vercel)
- [Future Improvements](#future-improvements)
- [Author](#author)
- [License](#license)

## 🎯 Project Overview

BuildMate is a Next.js application designed to empower developers and project managers with AI-driven capabilities. It combines Firebase for robust authentication and data management with Google's Gemini API to provide intelligent project suggestions and recommendations. The application features a modern, responsive user interface built with Tailwind CSS.

**Live Demo:** [https://build-mate-lemon.vercel.app](https://build-mate-lemon.vercel.app)

## ✨ Key Features

- **AI-Powered Suggestions** - Get intelligent project recommendations powered by Google Gemini API
- **User Authentication** - Secure Firebase authentication for user management
- **Real-time Database** - Cloud Firestore integration for persistent data storage
- **Responsive Design** - Mobile-first approach with Tailwind CSS styling
- **Type-Safe Development** - Full TypeScript support for robust code
- **Modern UI/UX** - Clean and intuitive user interface
- **Firestore Security Rules** - Robust security measures for data protection
- **Easy Deployment** - One-click deployment to Vercel

## 🛠 Tech Stack

| Technology | Purpose |
|-----------|---------|
| **Next.js 16** | React framework for production applications |
| **React 19** | UI library for building interactive components |
| **TypeScript 5** | Type-safe JavaScript development |
| **Tailwind CSS 3** | Utility-first CSS framework for styling |
| **Firebase 12** | Authentication and Firestore database |
| **Firebase Admin SDK 13** | Server-side Firebase operations |
| **Google Generative AI** | AI-powered suggestions via Gemini API |
| **Node.js** | JavaScript runtime environment |

## 📁 Folder Structure

```
BuildMate/
├── app/                    # Next.js App Router directory
│   ├── layout.tsx         # Root layout component
│   ├── page.tsx           # Home page
│   └── ...                # Other pages and routes
├── components/            # Reusable React components
│   ├── Header.tsx         # Header component
│   ├── ProjectCard.tsx    # Project card component
│   └── ...                # Other components
├── contexts/              # React Context for state management
│   └── AuthContext.tsx    # Authentication context
├── hooks/                 # Custom React hooks
│   ├── useAuth.ts         # Authentication hook
│   └── ...                # Other custom hooks
├── lib/                   # Utility functions and configurations
│   ├── firebase.ts        # Firebase configuration
│   ├── gemini.ts          # Gemini API integration
│   └── ...                # Other utilities
├── public/                # Static assets
├── styles/                # Global styles
├── .env.local.example     # Environment variables template
├── firebase.json          # Firebase configuration
├── firestore.rules        # Firestore security rules
├── firestore.indexes.json # Firestore indexes
├── next.config.js         # Next.js configuration
├── tailwind.config.js     # Tailwind CSS configuration
├── tsconfig.json          # TypeScript configuration
└── package.json           # Project dependencies
```

## 🔑 Environment Variables

Create a `.env.local` file in the root directory with the following variable:

```env
NEXT_PUBLIC_GEMINI_API_KEY=your_gemini_api_key_here
```

### Important Notes:
- The `NEXT_PUBLIC_` prefix makes this variable accessible in the browser
- Never commit your `.env.local` file to version control
- Keep your API keys confidential and rotate them regularly
- For Firebase configuration, ensure it's set up in your `lib/firebase.ts` file

## 📦 Installation

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn package manager
- Git

### Steps

1. **Clone the repository:**
```bash
git clone https://github.com/Adityaaryan1711/BuildMate.git
cd BuildMate
```

2. **Install dependencies:**
```bash
npm install
```

3. **Set up environment variables:**
```bash
# Copy the example file
cp .env.local.example .env.local

# Edit .env.local and add your Gemini API key
nano .env.local
```

4. **Configure Firebase (if needed):**
   - Update Firebase credentials in `lib/firebase.ts`
   - Ensure Firestore database is initialized in your Firebase project

## 🚀 How to Run Locally

1. **Start the development server:**
```bash
npm run dev
```

2. **Open your browser:**
   - Navigate to [http://localhost:3000](http://localhost:3000)
   - The application will automatically reload on file changes

3. **Available Scripts:**
   - `npm run dev` - Start development server
   - `npm run build` - Build for production
   - `npm start` - Start production server
   - `npm run lint` - Run ESLint for code quality

## 🌐 Deployment with Vercel

BuildMate is optimized for deployment on Vercel, providing a seamless CI/CD experience.

### Automatic Deployment (Recommended)

1. **Push your code to GitHub:**
```bash
git add .
git commit -m "Initial commit"
git push origin main
```

2. **Connect to Vercel:**
   - Visit [https://vercel.com](https://vercel.com)
   - Sign in with your GitHub account
   - Click "New Project"
   - Select your BuildMate repository
   - Vercel will auto-detect Next.js configuration

3. **Configure Environment Variables:**
   - In Vercel Dashboard, go to Settings → Environment Variables
   - Add `NEXT_PUBLIC_GEMINI_API_KEY`
   - Set the appropriate values for each environment (Production, Preview, Development)

4. **Deploy:**
   - Click "Deploy"
   - Vercel will automatically build and deploy your application

### Manual Deployment

1. **Install Vercel CLI:**
```bash
npm i -g vercel
```

2. **Deploy:**
```bash
vercel
```

3. **Follow the prompts** to complete the deployment

### Post-Deployment

- Your live URL will be provided (e.g., `https://buildmate-xxxxx.vercel.app`)
- Every push to the main branch triggers a new deployment
- Preview deployments are created for pull requests
- Check deployment logs in the Vercel Dashboard for troubleshooting

## 🎯 Future Improvements

- [ ] **Advanced Analytics** - Dashboard with project insights and metrics
- [ ] **Collaboration Features** - Real-time team collaboration and sharing
- [ ] **Project Templates** - Pre-built templates for common project types
- [ ] **Export Options** - Generate project files and documentation
- [ ] **API Documentation** - RESTful API for external integrations
- [ ] **Dark Mode Support** - Implement system-wide dark theme
- [ ] **Multi-language Support** - i18n internationalization
- [ ] **Advanced AI Features** - Code generation and architectural suggestions
- [ ] **Mobile App** - Native mobile applications (iOS/Android)
- [ ] **Integration Marketplace** - Connect with popular development tools
- [ ] **Offline Mode** - Progressive Web App (PWA) capabilities
- [ ] **Performance Optimization** - Image optimization and caching strategies

## 👨‍💻 Author

**Aditya Aryan**
- GitHub: [@Adityaaryan1711](https://github.com/Adityaaryan1711)
- Project Repository: [BuildMate](https://github.com/Adityaaryan1711/BuildMate)

## 📄 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

### Show Your Support ⭐

If you found this project helpful, please consider giving it a star on GitHub!

[Visit BuildMate on Vercel](https://build-mate-lemon.vercel.app)

</div>
