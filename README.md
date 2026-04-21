# Reinforce - Educational Platform

A modern educational course marketplace and learning platform built with vanilla JavaScript, HTML5, and CSS3. Reinforce provides a responsive, component-based architecture for showcasing courses, instructors, and micro-credentials.

## 🎯 Project Overview

Reinforce is a single-page application (SPA) designed to serve as an online learning platform where users can:
- Browse featured and trending courses
- View micro-credential programs
- Explore instructor profiles
- Access pricing information
- Sign up or log in to the platform

## 🏗️ Architecture

### Technology Stack
- **Frontend**: Vanilla JavaScript (ES6+)
- **Markup**: HTML5
- **Styling**: CSS3 with CSS variables
- **Build**: No build process required - runs directly in the browser

### Design Pattern
- **Component-based architecture**: Modular, reusable UI components
- **Dynamic mounting**: Components are fetched and rendered at runtime into designated mount points
- **Theme system**: Light/Dark mode with localStorage persistence
- **Responsive design**: Mobile-first approach with hamburger menu for mobile navigation

## 📁 Project Structure

```
reinforceDemo/
├── index.html              # Home page entry point
├── index.js                # Home page initialization & component mounting
├── README.md               # This file
├── assets/                 # Static resources
│   ├── images/             # Logo, course images, instructor images
│   ├── js/                 # Shared scripts (theme.js)
│   ├── styles/             # Global CSS
│   └── videos/             # Video assets
├── components/             # Reusable UI components
│   ├── header/             # Navigation header with mobile menu
│   ├── hero/               # Hero banner section
│   ├── featured-courses/   # Featured courses showcase
│   ├── top-courses-week/   # Weekly trending courses
│   ├── micro-credential-courses/  # Certification programs
│   ├── instructors-preview/       # Featured instructors
│   ├── testimonials/       # User testimonials
│   ├── enrollment-cta/     # Call-to-action section
│   ├── trusted-by/         # Partner logos
│   └── footer/             # Footer with links
└── pages/                  # Multi-page routes
    ├── home/               # Home page components
    ├── course-details/     # Course detail page
    ├── instructor-details/ # Instructor profile page
    ├── pricing/            # Pricing page
    └── auth/               # Authentication (Sign Up / Log In)
```

## 🎨 Key Features

### 1. **Theme System**
- Light and Dark mode support
- Persistent theme selection using localStorage
- Material Design 3 inspired color palette
- CSS variables for easy customization

### 2. **Responsive Components**
- Mobile-friendly hamburger menu
- Adaptive layouts for all screen sizes
- Touch-friendly interface

### 3. **Component Reusability**
- Shared header and footer across pages
- Modular CSS and HTML files
- Consistent styling and behavior

### 4. **Animations & Interactions**
- Smooth scroll reveal animations
- Intersection Observer API for performance-optimized animations
- Theme toggle transitions

### 5. **Dynamic Content Loading**
- Components fetched from separate HTML files
- Path normalization for proper asset loading
- Error handling for failed component loads

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Local web server (required for fetch API to work)

### Setup

1. **Clone or download the project**
   ```bash
   git clone <repository-url>
   cd reinforceDemo
   ```

2. **Start a local web server**
   
   Using Python:
   ```bash
   python -m http.server 8000
   ```
   
   Using Node.js (http-server):
   ```bash
   npx http-server -p 8000
   ```
   
   Using Live Server in VS Code:
   - Install "Live Server" extension
   - Right-click index.html → "Open with Live Server"

3. **Open in browser**
   - Navigate to `http://localhost:8000/reinforceDemo/`

## 🎯 Component Guide

### Header
- Navigation bar with logo and menu
- Mobile hamburger menu with responsive toggle
- Location: `components/header/`

### Hero Section
- Eye-catching banner with call-to-action
- Location: `components/hero/`

### Course Sections
- **Featured Courses**: Curated course selection
- **Top Courses Week**: Trending courses
- **Micro-Credential Courses**: Certification programs
- Location: `components/*/`

### Instructors
- Preview of featured instructors
- Location: `components/instructors-preview/`

### Testimonials
- User reviews and feedback
- Location: `components/testimonials/`

### Footer
- Links and copyright information
- Location: `components/footer/`

## 🎨 Styling

### CSS Variables
Global variables defined in `assets/styles/global.css`:
- **Colors**: Primary blue (#a7c8fc), Secondary teal (#9ed1c6)
- **Typography**: Font families and sizes
- **Spacing**: Margins and padding scales
- **Breakpoints**: Responsive design breakpoints

### Theme Customization
Edit CSS variables in `global.css` to customize:
- Brand colors
- Font sizes
- Spacing values
- Dark/Light mode colors

## 📄 Pages

### Home (`index.html`)
- Landing page showcasing all platform features
- Component mounting points for dynamic content

### Course Details (`pages/course-details/`)
- Detailed course information
- Instructor bio
- Enrollment options

### Instructor Details (`pages/instructor-details/`)
- Instructor profile and bio
- List of courses taught
- Contact information

### Pricing (`pages/pricing/`)
- Subscription plans
- Feature comparison
- Pricing details

### Authentication (`pages/auth/`)
- User sign-up / log-in
- User type selection (Student/Instructor)

## 🔧 Development

### Adding a New Component

1. Create a folder in `components/`
2. Create HTML file with the component markup
3. Create CSS file with component styles
4. Create JavaScript file if needed for interactions
5. Add mount point in the parent page
6. Load in the parent page's JavaScript file

### Adding a New Page

1. Create folder in `pages/`
2. Create `index.html` with page structure
3. Create `index.js` for page initialization
4. Create CSS file for page-specific styles
5. Add appropriate mount points for shared components

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 📝 Notes

- The project uses the Fetch API, requiring a local web server for development
- All assets are relative paths; ensure proper path handling when deploying
- Mobile menu state is managed in `components/header/header-mobile-menu.js`
- Theme preference is stored in browser's localStorage

## 🤝 Contributing

When contributing:
1. Maintain component modularity
2. Follow existing naming conventions
3. Update CSS variables for consistent theming
4. Test on mobile and desktop viewports
5. Ensure all components are accessible

