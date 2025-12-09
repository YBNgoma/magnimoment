# Magnimoments

A beautiful, modern web application for creating and managing digital memorial pages. Preserve memories, share photos, and celebrate the lives of loved ones with an elegant, role-based platform.

## Features

- **🏛️ Digital Memorials**: Create stunning memorial pages with photos, bios, and timelines
- **👥 Role-Based Access**: Three permission levels (Super Admin, Owner, Contributor)
- **📸 Photo Sharing**: Upload and organize photos with AI-suggested tags and captions
- **🔐 Authentication**: Simple email-based login system
- **💾 Local Storage**: All data persists in browser localStorage (demo mode)
- **✨ Beautiful UI**: Premium design with Tailwind CSS, smooth animations, and responsive layouts

## Tech Stack

- **Frontend**: React 19 + TypeScript
- **Build Tool**: Vite 6
- **Styling**: Tailwind CSS (via CDN)
- **Icons**: Lucide React
- **State Management**: React hooks + localStorage

## Getting Started

### Prerequisites

- Node.js 18+
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd magnimoments
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser** to `http://localhost:3000`

### Demo Accounts

For testing, use these email addresses:

- **Super Admin**: `admin@magnimoments.com`
- **Regular User**: `jane@family.com` or `mike@family.com`
- **Or enter any email** to auto-create a new user

## Deployment

### Deploy to Cloudflare Pages

This project is configured for easy deployment to Cloudflare Pages using Wrangler:

1. **Build and deploy**
   ```bash
   npm run deploy
   ```

2. **Authenticate** (first time only)
   Follow the prompts to log in to your Cloudflare account

3. **Live!** Your app will be deployed and accessible via Cloudflare Pages

## Project Structure

```
magnimoments/
├── components/       # Reusable UI components
├── pages/           # Main application pages
│   ├── Auth.tsx     # Login/authentication
│   ├── Dashboard.tsx # Memorial list and management
│   └── Memorial.tsx  # Individual memorial page
├── services/        # Backend logic and data management
│   ├── mockBackend.ts   # LocalStorage-based backend
│   └── geminiService.ts # AI integration for photo analysis
├── types.ts         # TypeScript type definitions
└── App.tsx          # Main application component
```

## How It Works

1. **Login**: Users authenticate with their email (demo mode auto-creates accounts)
2. **Dashboard**: View memorials you have access to based on your role
3. **Create Memorial**: Super admins can create new memorial pages and assign owners
4. **Manage Access**: Owners can invite contributors to share photos and memories
5. **Add Photos**: All users with access can upload and tag photos

## License

This project is open source and available under the MIT License.

---

Built with ❤️ to preserve precious memories
