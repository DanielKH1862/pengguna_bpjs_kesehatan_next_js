# 🏥 BPJS Kesehatan - Portal Anggota

A modern, accessible, and user-friendly web application for BPJS Kesehatan (Indonesian Health Insurance) member portal. Built with Next.js 14 and designed with accessibility and elderly users in mind.

## ✨ Features

### 🔐 Authentication
- **Secure Login** with NIK/User ID and password validation
- **Biometric Authentication** support (Fingerprint & Face ID)
- **Multi-step Registration** with 4-step visual progress indicator
- **Email Verification** and account confirmation
- **Password Recovery** functionality
- **Enhanced Security** with data protection notices

### 📊 Dashboard
- **Member Information** display with real-time status indicators
- **Payment Status** tracking with visual progress bars
- **Health Quota** monitoring with detailed usage statistics
- **Quick Access** to essential healthcare services
- **Recent Activities** timeline with status indicators
- **Responsive Design** optimized for all devices
- **Interactive Cards** with hover effects and animations

### 🎨 Design System
- **Accessibility-First** design specifically for elderly users
- **High Contrast** color schemes with WCAG 2.1 AA compliance
- **Large Text Options** with `.text-elderly` and `.text-elderly-large` classes
- **Touch-Friendly** interfaces with enhanced touch targets
- **Professional UI/UX** with modern design patterns and micro-interactions
- **Consistent Branding** with official BPJS Kesehatan colors
- **Gradient Backgrounds** and modern visual effects

### 🚀 Technical Features
- **Next.js 14** with App Router and modern React patterns
- **Tailwind CSS** with custom design system
- **Responsive Design** (Mobile-first approach)
- **Component-Based Architecture** with reusable UI components
- **Modern JavaScript (ES6+)** with hooks and functional components
- **Enhanced Accessibility** with ARIA labels and keyboard navigation

## 🛠️ Tech Stack

- **Framework:** Next.js 14
- **Styling:** Tailwind CSS
- **Icons:** Heroicons (SVG)
- **Fonts:** Inter & Poppins (Google Fonts)
- **Deployment:** Vercel (recommended)

## 📁 Project Structure

```
bpjs_kesehatan/
├── public/                          # Static assets
│   ├── file.svg
│   ├── globe.svg
│   ├── next.svg
│   ├── vercel.svg
│   └── window.svg
├── src/
│   └── app/                         # Next.js App Router
│       ├── components/              # Reusable UI components
│       │   └── ui/
│       │       ├── button/
│       │       │   └── page.js      # Button component demo
│       │       ├── Button.js        # Enhanced Button component with variants
│       │       ├── Card.js          # Card component with Header/Content/Footer
│       │       ├── Input.js         # Input component with validation & accessibility
│       │       └── ProgressBar.js   # Progress bar for multi-step forms
│       ├── favicon.ico              # Site favicon
│       ├── globals.css              # Global styles, CSS variables & accessibility
│       ├── layout.js                # Root layout with metadata
│       ├── page.js                  # Main dashboard (authenticated users)
│       ├── login/                   # Authentication pages
│       │   └── page.js              # Login with biometric options
│       ├── register/                # Registration flow
│       │   └── page.js              # 4-step registration process
│       └── register-lanjutan/       # Extended registration
│           └── page.js              # Additional user information
├── .gitignore                       # Git ignore rules
├── eslint.config.mjs                # ESLint configuration
├── jsconfig.json                    # JavaScript configuration
├── next.config.mjs                  # Next.js configuration
├── package.json                     # Dependencies and scripts
├── package-lock.json                # Lock file for dependencies
├── postcss.config.mjs               # PostCSS configuration
└── README.md                        # Project documentation
```

### 📂 Key Directories Explained

- **`src/app/`** - Next.js 14 App Router directory
- **`src/app/components/ui/`** - Reusable UI components with enhanced accessibility
- **`src/app/login/`** - Authentication pages with biometric support
- **`src/app/register/`** - Multi-step registration with progress tracking
- **`src/app/register-lanjutan/`** - Extended registration for additional user data
- **`public/`** - Static assets and icons

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd bpjs_kesehatan
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Run the development server**
```bash
npm run dev
# or
yarn dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🎨 Design System

### Color Palette
- **Primary:** `#00A86B` (BPJS Green)
- **Primary Dark:** `#007A4F`
- **Primary Light:** `#E8F5F0`
- **Primary Lighter:** `#F0F9F5`
- **Secondary:** `#2E7D32`
- **Accent:** `#4CAF50`
- **Accent Light:** `#81C784`

### Enhanced Color System
- **Success:** `#059669` with light variant `#D1FAE5`
- **Warning:** `#D97706` with light variant `#FEF3C7`
- **Error:** `#DC2626` with light variant `#FEE2E2`
- **Info:** `#2563EB` with light variant `#DBEAFE`

### Typography
- **Primary Font:** Inter (Body text) - 300, 400, 500, 600, 700, 800 weights
- **Heading Font:** Poppins (Titles and headings) - 300, 400, 500, 600, 700, 800 weights
- **Font Sizes:** Responsive scale from 0.75rem to 4rem
- **Line Heights:** Optimized for readability (1.3-1.8)

### Accessibility Features
- **High Contrast Mode** support with `@media (prefers-contrast: high)`
- **Large Text Options** for elderly users (`.text-elderly`, `.text-elderly-large`)
- **Enhanced Focus States** with 3px outline and rounded corners
- **Screen Reader** friendly markup with `.sr-only` class
- **Keyboard Navigation** support with proper tab order
- **Reduced Motion** support with `@media (prefers-reduced-motion: reduce)`
- **Touch Targets** minimum 44px for mobile accessibility

## 📱 Pages Overview

### 🔐 Login Page (`/login`)
- **Enhanced Authentication** with NIK/User ID and password validation
- **Biometric Options** for Fingerprint and Face ID login
- **Security Features** with "Remember me" functionality
- **Password Recovery** link and security notices
- **Accessibility** with large text options and high contrast
- **Visual Design** with gradient backgrounds and modern UI

### 📝 Registration Page (`/register`)
- **4-Step Process** with visual progress indicator:
  1. **Personal Information** - NIK, name, email, phone, birth details
  2. **Address Information** - Complete address with validation
  3. **Account Setup** - Password creation with strength indicators
  4. **Confirmation** - Success page with next steps
- **Real-time Validation** with helpful error messages
- **Enhanced UX** with step icons and clear navigation
- **Accessibility** optimized for elderly users

### 🏥 Dashboard (`/`)
- **Welcome Section** with animated gradient background
- **Member Information** card with status indicators
- **Payment Status** with visual progress and amount display
- **Health Quota** tracking with usage statistics and progress bars
- **Quick Access** to 6 essential healthcare services
- **Recent Activities** timeline with status badges
- **Responsive Sidebar** with enhanced navigation
- **Interactive Elements** with hover effects and animations

### 📋 Extended Registration (`/register-lanjutan`)
- **Additional Information** collection
- **Health Data** including blood type and medical history
- **Preferences** for healthcare services
- **Notification Settings** for email, SMS, and WhatsApp

## 🧩 Components

### Button Component
Enhanced button with multiple variants and accessibility features:
```jsx
<Button 
  variant="primary"        // primary, secondary, outline, ghost, danger, success
  size="lg"               // sm, md, lg, xl
  className="btn-high-contrast"
  disabled={false}
  type="button"
>
  Click Me
</Button>
```

### Input Component
Accessible input with validation and password toggle:
```jsx
<Input
  label="Email"
  type="email"
  placeholder="Enter your email"
  required
  showPasswordToggle      // For password fields
  error={errorMessage}    // Display validation errors
  helperText="Helper text"
  className="input-enhanced text-large"  // Enhanced styling
/>
```

### Card Component
Flexible card with header, content, and footer sections:
```jsx
<Card className="card-enhanced hover:shadow-lg">
  <Card.Header className="pb-6">
    <h2>Card Title</h2>
  </Card.Header>
  <Card.Content>
    <p>Card content goes here</p>
  </Card.Content>
  <Card.Footer>
    <Button>Action</Button>
  </Card.Footer>
</Card>
```

### Progress Bar Component
Multi-step progress indicator:
```jsx
<ProgressBar 
  steps={4} 
  currentStep={2} 
  className="mb-8"
/>
```

## 🎯 Key Features

### For Elderly Users
- **Large Text Options:** `.text-elderly` and `.text-elderly-large` classes
- **Enhanced Touch Targets:** Minimum 44px touch areas with `.elderly-friendly` class
- **High Contrast:** Better visibility with enhanced color contrast ratios
- **Simple Navigation:** Clear, intuitive interface with large buttons
- **Clear Visual Feedback:** Obvious success/error states with color coding
- **Reduced Motion:** Support for users who prefer less animation
- **Voice-Friendly:** Proper ARIA labels for screen readers

### For All Users
- **Responsive Design:** Mobile-first approach that works on all screen sizes
- **Fast Loading:** Optimized performance with modern React patterns
- **Modern UI:** Contemporary design with gradients and micro-interactions
- **Accessibility:** WCAG 2.1 AA compliant with comprehensive testing
- **Security:** Secure authentication flow with biometric options
- **Progressive Enhancement:** Works without JavaScript for basic functionality

## 🔧 Configuration

### Environment Variables
Create a `.env.local` file in the root directory:

```env
NEXT_PUBLIC_APP_NAME="BPJS Kesehatan"
NEXT_PUBLIC_APP_VERSION="1.0.0"
# Add your API endpoints and keys here
```

### Tailwind Configuration
The project uses a custom Tailwind configuration with:
- BPJS brand colors
- Custom spacing and typography
- Accessibility-focused utilities
- Component-specific classes

## 📦 Available Scripts

```bash
# Development
npm run dev          # Start development server
npm run build        # Build for production
npm run start        # Start production server
npm run lint         # Run ESLint

# Code Quality
npm run lint:fix     # Fix ESLint errors
npm run type-check   # Run TypeScript checks (if using TS)
```

## 🚀 Deployment

### Vercel (Recommended)
1. Push your code to GitHub
2. Connect your repository to Vercel
3. Deploy automatically on every push

### Other Platforms
- **Netlify:** Compatible with Next.js
- **AWS Amplify:** Full-stack deployment
- **Docker:** Containerized deployment

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support and questions:
- Create an issue in the repository
- Contact the development team
- Check the documentation

## 🔄 Version History

### v1.0.0 (Current) - Enhanced UI/UX Release
- **Complete Authentication Flow** with biometric support
- **4-Step Registration Process** with visual progress tracking
- **Enhanced Dashboard** with interactive cards and animations
- **Comprehensive Accessibility** features for elderly users
- **Mobile-First Responsive Design** optimized for all devices
- **Modern UI/UX** with gradients, micro-interactions, and professional design
- **Enhanced Design System** with improved color palette and typography
- **Health Quota Tracking** with visual progress bars and statistics
- **Interactive Components** with hover effects and smooth transitions
- **Security Enhancements** with data protection notices and secure forms

## 🆕 Recent Improvements

### UI/UX Enhancements
- **Enhanced Login Page** with biometric authentication options
- **Improved Registration Flow** with 4-step process and success confirmation
- **Redesigned Dashboard** with modern cards and interactive elements
- **Accessibility Improvements** with elderly-friendly features
- **Mobile Optimization** with responsive design patterns
- **Visual Design Updates** with gradients, shadows, and animations

### Technical Improvements
- **Enhanced CSS Variables** for better color management
- **Improved Component Architecture** with better accessibility
- **Form Validation** with real-time feedback
- **Loading States** with professional animations
- **Error Handling** with user-friendly messages

## 🙏 Acknowledgments

- **BPJS Kesehatan** for the design requirements and healthcare focus
- **Next.js Team** for the amazing React framework
- **Tailwind CSS** for the utility-first CSS framework
- **Heroicons** for the beautiful SVG icons
- **Google Fonts** for Inter and Poppins typography
- **Accessibility Community** for WCAG guidelines and best practices

---

**Built with ❤️ for better healthcare access in Indonesia**

*This application prioritizes accessibility and user experience to ensure all Indonesians can easily access their healthcare benefits through BPJS Kesehatan.*
