# Urbia Spatial Manifesto

Welcome to the official repository for **Urbia**, a web platform showcasing spatial design, community building initiatives, and the collective's portfolio.

## � Mission Statement
Urbia is a spatial design collective dedicated to manifesting new forms of urban living. This platform serves as a digital manifesto, showcasing our projects, services, and community-building efforts. It connects visitors with our work and philosophy through an immersive and responsive user experience.

## ✨ Key Features
- **Dynamic Homepage**: Immersive landing page with a full-screen carousel (`HomeCarousel`) and introduction.
- **Project Showcase**: A dedicated section to display our portfolio (`/projects`), managed via Contentful CMS.
- **Services Overview**: Detailed breakdown of services provided by Urbia (`/services`).
- **Community Engagement**: Information on community building initiatives (`/build-community`).
- **Team Page**: Meet the team behind Urbia ("We Are Urbians!" at `/urbians`).
- **Contact & Inquiry**: Integrated contact forms powered by Formspree.
- **Responsive Design**: Fully responsive layout optimized for mobile and desktop using **Tailwind CSS**.
- **Interactive UI**: Animated components and smooth transitions powered by Framer Motion / CSS animations.

## 🛠 Tech Stack
This project is built with a modern, performance-focused stack:

**Core:**
- [Next.js 14](https://nextjs.org/) (App Router)
- [React](https://react.dev/)
- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

**Styling & UI:**
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework.
- [Radix UI](https://www.radix-ui.com/) - Unstyled, accessible UI primitives (Accordion, Select, etc.).
- [FontAwesome](https://fontawesome.com/) & [React Icons](https://react-icons.github.io/react-icons/) - Iconography.

**Content & Data:**
- [Contentful](https://www.contentful.com/) - Headless CMS for managing dynamic content like projects.
- [Formspree](https://formspree.io/) - Form handling service.

## 🚀 Getting Started

### Prerequisites
Ensure you have the following installed:
- **Node.js** (v18+ recommended)
- **npm** or **yarn** or **pnpm** (pnpm is used in the lockfile)

### Setup Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd urbia
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   pnpm install
   ```

3. **Configure Environment Variables**
   Create a `.env.local` file in the root directory and add your Contentful and other API keys:
   ```env
   CONTENTFUL_SPACE_ID=your_space_id
   CONTENTFUL_ACCESS_TOKEN=your_access_token
   NEXT_PUBLIC_FORMSPREE_ID=your_formspree_id
   ```

4. **Launch Development Server**
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## 📜 Essential Scripts

- `npm run dev`: Starts the local development server.
- `npm run build`: Builds the application for production.
- `npm run start`: Starts the production server.
- `npm run lint`: Runs ESLint to check for code quality issues.
- `npm run setup`: Runs the project setup script.

## 📂 Project Structure

```
src/
├── app/                 # Next.js App Router pages (routes)
│   ├── build-community/ # Community page
│   ├── posts/           # Blog/Article posts
│   ├── projects/        # Projects portfolio
│   ├── services/        # Services offered
│   ├── urbians/         # Team/About page
│   └── page.js          # Main entry (Homepage wrapper)
├── components/          # Reusable UI components
│   ├── ui/              # Primitive components (Navbar, Button, etc.)
│   └── ...              # Complex modules (Header, Footer, Carousel)
├── homepage/            # Homepage specific components
└── lib/                 # Utility functions and API clients (Contentful)
```

## 📚 Internal Documentation
For more details on specific implementations, refer to the code within `src/lib/api.js` for Contentful integration and individual component files for UI logic.