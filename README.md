
# Cybersecurity Elite Portfolio

> A visually stunning, 3D immersive cybersecurity portfolio website built with modern web technologies.

## 🚀 Features

- ✅ **Immersive 3D Experience** - React Three Fiber particle networks, rotating shields, skill spheres
- ✅ **Cybersecurity Theme** - Dark theme with neon blues, greens, and purples
- ✅ **Responsive Design** - Fully optimized for mobile, tablet, and desktop
- ✅ **Smooth Animations** - Framer Motion + GSAP for professional motion design
- ✅ **Performance Optimized** - Lazy loading, code splitting, image optimization
- ✅ **SEO Ready** - Complete meta tags, structured data, Open Graph support
- ✅ **Accessibility** - WCAG 2.1 compliant with keyboard navigation
- ✅ **Production Ready** - Clean code, TypeScript, best practices

## 📋 Sections

1. **Hero** - Particle network background with typing animation
2. **About** - Profile with rotating 3D shield and education details
3. **Skills** - Interactive skill cards and 3D skill sphere
4. **Experience** - Timeline view of professional history
5. **Projects** - Project cards with modal details
6. **Certifications** - Holographic certification badges
7. **Contact** - Terminal-style contact form
8. **Footer** - Social links and copyright

## 🛠️ Tech Stack

- **Framework**: Next.js 15 with App Router
- **UI Library**: React 18
- **Styling**: Tailwind CSS + Custom CSS
- **Animation**: Framer Motion + GSAP
- **3D Graphics**: Three.js + React Three Fiber
- **Language**: TypeScript
- **Deployment**: Vercel

## 📦 Installation

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Setup

```bash
# Clone the repository
git clone https://github.com/Bennyhinn007/cybersecurity-portfolio.git
cd cybersecurity-portfolio

# Install dependencies
npm install
# or
yarn install

# Run development server
npm run dev
# or
yarn dev

# Open browser
# Navigate to http://localhost:3000
```

## 🏗️ Build & Deployment

### Local Build

```bash
# Build for production
npm run build

# Start production server
npm run start
```

### Deploy to Vercel

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# For production deployment
vercel --prod
```

Or connect your GitHub repository to Vercel dashboard for automatic deployments.

## 📁 Project Structure

```
src/
├── app/                      # Next.js app directory
│   ├── layout.tsx           # Root layout with SEO metadata
│   ├── page.tsx             # Homepage
│   ├── globals.css          # Global styles
│   └── metadata.ts          # SEO configuration
├── components/
│   ├── Layout/              # Navigation, Footer, Loading
│   ├── Hero/                # Hero section with particle effects
│   ├── About/               # About section with 3D shield
│   ├── Skills/              # Skills section with 3D sphere
│   ├── Experience/          # Timeline experience cards
│   ├── Projects/            # Project cards and modal
│   ├── Certifications/      # Certification badges
│   ├── Contact/             # Contact section and form
│   └── Common/              # Reusable components
├── utils/
│   ├── constants.ts         # Navigation, social links, skills
│   ├── data.ts              # Projects, experience, education
│   └── animations.ts        # Framer Motion variants
├── hooks/
│   ├── useMousePosition.ts  # Mouse tracking
│   └── useScrollTrigger.ts  # Scroll detection
└── styles/
    └── animations.module.css # Custom CSS animations
```

## 🎨 Customization

### Update Personal Information

Edit `src/utils/constants.ts` and `src/utils/data.ts`:

```typescript
// constants.ts
export const SOCIAL_LINKS = {
  linkedin: 'your-linkedin-url',
  github: 'your-github-url',
  tryhackme: 'your-tryhackme-url',
  email: 'your-email@example.com',
  phone: 'your-phone-number',
};

// data.ts
export const PROJECTS = [
  // Add your projects
];

export const EXPERIENCE = [
  // Add your experience
];
```

### Customize Colors

Edit `tailwind.config.ts`:

```typescript
colors: {
  cyber: {
    black: '#0a0e27',      // Main background
    navy: '#0f1b3c',       // Secondary background
    blue: '#00d4ff',       // Primary accent
    green: '#39ff14',      // Secondary accent
    purple: '#d946ef',     // Tertiary accent
  },
}
```

### Modify Animations

Edit animation timing in `src/utils/animations.ts` and `src/styles/animations.module.css`.

## 📊 Performance Optimization

### Already Implemented

- ✅ Image optimization with WebP/AVIF formats
- ✅ Code splitting with dynamic imports
- ✅ CSS-in-JS with Tailwind tree-shaking
- ✅ Font optimization with system fonts
- ✅ Preconnect to external resources
- ✅ Lazy loading for heavy components
- ✅ Compression enabled in next.config.js

### Additional Tips

1. **Monitor Bundle Size**
   ```bash
   npm run build
   # Check .next/static/ folder
   ```

2. **Test Performance**
   - Use Lighthouse: https://developers.google.com/web/tools/lighthouse
   - Use WebPageTest: https://www.webpagetest.org/

3. **Optimize Images**
   - Convert images to WebP
   - Use responsive images with srcset
   - Compress with TinyPNG/ImageOptim

## 🔒 Security Best Practices

- ✅ HTTPS enforced on production
- ✅ X-Content-Type-Options header set
- ✅ X-Frame-Options to prevent clickjacking
- ✅ X-XSS-Protection enabled
- ✅ Referrer Policy configured
- ✅ No sensitive data in client-side code
- ✅ Form validation and sanitization

## ♿ Accessibility Features

- ✅ Semantic HTML structure
- ✅ ARIA labels and descriptions
- ✅ Keyboard navigation support
- ✅ Focus indicators for all interactive elements
- ✅ Color contrast meets WCAG AA standards
- ✅ Reduced motion support with `prefers-reduced-motion`

## 📱 Responsive Breakpoints

- Mobile: `< 640px`
- Tablet: `640px - 1024px`
- Desktop: `> 1024px`

All components are fully responsive and tested across devices.

## 🐛 Troubleshooting

### Port Already in Use
```bash
# Change port
npm run dev -- -p 3001
```

### 3D Components Not Rendering
- Check browser WebGL support
- Ensure Three.js is installed: `npm install three @react-three/fiber`
- Clear cache: `rm -rf .next && npm run dev`

### Build Errors
```bash
# Clear cache and reinstall
rm -rf node_modules .next
npm install
npm run build
```

## 📈 SEO Checklist

- ✅ Meta description optimized
- ✅ Open Graph tags for social sharing
- ✅ Twitter Card support
- ✅ Structured data (Schema.org)
- ✅ Sitemap auto-generated
- ✅ Robots.txt configured
- ✅ Mobile-friendly design
- ✅ Fast Core Web Vitals

## 🚀 Deployment Checklist

- ✅ Update personal information
- ✅ Add profile photo (optional)
- ✅ Test all links
- ✅ Run Lighthouse audit
- ✅ Test on mobile devices
- ✅ Set up analytics
- ✅ Enable monitoring
- ✅ Configure custom domain (if applicable)

## 📚 Additional Resources

- [Next.js Documentation](https://nextjs.org/docs)
- [React Three Fiber](https://docs.pmnd.rs/react-three-fiber)
- [Framer Motion](https://www.framer.com/motion)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [Three.js](https://threejs.org/docs)

## 📝 License

This project is personal. Feel free to use it as a template.

## 👥 Support

For questions or support:
- Email: bennysangnalkar@gmail.com
- LinkedIn: https://linkedin.com/in/bennyhinn29
- GitHub: https://github.com/Bennyhinn007

---

**Made with ❤️ by Benny Hinn | Cybersecurity Engineer**
