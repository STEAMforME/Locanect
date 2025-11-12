// README.md content displayed as a formatted documentation page

const README_CONTENT = `
# Locanect - Civic Tech Platform

## 🚀 Production-Ready Landing Page & Core UI

Locanect is a civic-tech platform that connects residents to vital local services—housing assistance, youth programs, reentry support, and more—without the runaround.

---

## 📋 Features

### Pages
- **Landing (/)**: Hero with call-to-action buttons, smooth scroll to forms
- **About (/about)**: Origin story and three icon cards (Mission, Vision, Community Roots)
- **Services (/services)**: Grid of five core services with descriptions
- **Partners (/partners)**: Logo wall and validated partner inquiry form
- **Contact (/contact)**: Beta signup form with validation

### Components
- **Navbar**: Responsive navigation with language toggle stub (EN/ES)
- **Footer**: Civic-friendly footer with quick links
- **CallToAction**: Primary action buttons
- **PartnerForm**: Validated form for organizations (Formspree integration)
- **BetaForm**: Beta signup with city dropdown, role selection, interest tags

### Technical Features
- ✅ React 18 with modern hooks
- ✅ React Router v6 with five routes
- ✅ Tailwind CSS for responsive, mobile-first design
- ✅ Scroll-based reveal animations (Intersection Observer)
- ✅ WCAG-compliant color contrast and focus states
- ✅ Form validation with user feedback
- ✅ Smooth scrolling to form sections
- ✅ Fully responsive (mobile, tablet, desktop)

---

## 🛠️ Tech Stack

- **Framework**: React 18
- **Build Tool**: Vite (simulated via CDN for this demo)
- **Styling**: Tailwind CSS (JIT mode)
- **Routing**: React Router v6
- **Animations**: Custom Intersection Observer hooks
- **Forms**: Formspree integration (placeholder endpoints)
- **Fonts**: Inter (Google Fonts)

---

## 📦 Installation & Setup

### Prerequisites
- Node.js 16+ and npm/yarn

### Local Development

\`\`\`bash
# Clone the repository
git clone https://github.com/your-org/locanect.git
cd locanect

# Install dependencies
npm install
# or
yarn install

# Start development server
npm run dev
# or
yarn dev
\`\`\`

The app will be available at \`http://localhost:5173\`

### Build for Production

\`\`\`bash
npm run build
# or
yarn build
\`\`\`

Production files will be in the \`dist/\` directory.

---

## 🚢 Deployment

### Vercel (Recommended)

1. **Install Vercel CLI**:
   \`\`\`bash
   npm install -g vercel
   \`\`\`

2. **Deploy**:
   \`\`\`bash
   vercel
   \`\`\`

3. **Follow prompts** to link your project and deploy

**Or use Vercel Dashboard**:
1. Push code to GitHub
2. Visit [vercel.com](https://vercel.com)
3. Click "New Project"
4. Import your GitHub repository
5. Vercel auto-detects Vite and configures everything
6. Click "Deploy"

### Netlify

\`\`\`bash
# Install Netlify CLI
npm install -g netlify-cli

# Build and deploy
npm run build
netlify deploy --prod --dir=dist
\`\`\`

### GitHub Pages

\`\`\`bash
# Build
npm run build

# Deploy (requires gh-pages package)
npm install -D gh-pages
npx gh-pages -d dist
\`\`\`

---

## 📁 Project Structure

\`\`\`
locanect/
├── src/
│   ├── components/
│   │   ├── Navbar.jsx
│   │   ├── Footer.jsx
│   │   ├── CallToAction.jsx
│   │   ├── PartnerForm.jsx
│   │   └── BetaForm.jsx
│   ├── pages/
│   │   ├── LandingPage.jsx
│   │   ├── AboutPage.jsx
│   │   ├── ServicesPage.jsx
│   │   ├── PartnersPage.jsx
│   │   └── ContactPage.jsx
│   ├── hooks/
│   │   └── useInView.js
│   ├── App.jsx
│   └── main.jsx
├── public/
├── index.html
├── package.json
├── vite.config.js
├── tailwind.config.js
├── postcss.config.js
└── README.md
\`\`\`

---

## 🎨 Design System

### Colors
- **Primary**: Blue-600 (\`#2563eb\`)
- **Background**: Gray-50 (\`#f9fafb\`)
- **Text**: Gray-900 (\`#111827\`)
- **Accent Colors**: Green, Yellow, Purple, Red for service cards

### Typography
- **Font Family**: Inter, Lato (with system fallbacks)
- **Weights**: 400 (regular), 500 (medium), 600 (semibold), 700 (bold)

### Breakpoints
- **Mobile**: < 640px
- **Tablet**: ≥ 640px
- **Desktop**: ≥ 1024px

---

## 📝 Form Configuration

### Formspree Setup

Replace placeholder endpoints in the code:

1. **Partner Form** (\`PartnerForm.jsx\`):
   \`\`\`javascript
   fetch('https://formspree.io/f/YOUR_FORM_ID', { ... })
   \`\`\`

2. **Beta Form** (\`BetaForm.jsx\`):
   \`\`\`javascript
   fetch('https://formspree.io/f/YOUR_BETA_FORM_ID', { ... })
   \`\`\`

### Get Formspree IDs:
1. Sign up at [formspree.io](https://formspree.io)
2. Create two forms (Partner & Beta)
3. Copy the form IDs
4. Replace in the component files

---

## ♿ Accessibility

- ✅ WCAG 2.1 AA compliant color contrast
- ✅ Focus indicators on all interactive elements
- ✅ Semantic HTML structure
- ✅ ARIA labels where appropriate
- ✅ Keyboard navigation support
- ✅ Screen reader friendly

---

## 🌐 Language Toggle

The language toggle (EN/ES) is currently a **stub** for future implementation. To implement:

1. Use a library like \`react-i18next\`
2. Create translation files (\`en.json\`, \`es.json\`)
3. Wire up the toggle button to switch languages
4. Wrap text content with translation functions

---

## 🧪 Testing Locally

1. **Test all routes**:
   - / (Landing)
   - /about
   - /services
   - /partners
   - /contact

2. **Test responsive design**:
   - Mobile (< 640px)
   - Tablet (640px - 1024px)
   - Desktop (> 1024px)

3. **Test forms**:
   - Validation (required fields, email format)
   - Submission (check Formspree dashboard)
   - Success states

4. **Test accessibility**:
   - Tab through all interactive elements
   - Check focus indicators
   - Use screen reader (optional)

---

## 🤝 Contributing

Locanect is built for the community, by the community. Contributions welcome!

1. Fork the repository
2. Create a feature branch (\`git checkout -b feature/amazing-feature\`)
3. Commit changes (\`git commit -m 'Add amazing feature'\`)
4. Push to branch (\`git push origin feature/amazing-feature\`)
5. Open a Pull Request

---

## 📄 License

MIT License - feel free to use this for your civic tech projects!

---

## 📞 Support

- **Email**: hello@locanect.org
- **Phone**: (555) 123-4567
- **Serving**: Newark, Irvington, Camden, New Brunswick, Detroit

---

## 🙏 Acknowledgments

- **STEAM for ME**: Our founding partner organization
- **Community organizers** in Newark and partner cities
- **Residents** who shared their experiences and needs

---

**Built with ❤️ for communities everywhere**
`;

// Display README as formatted HTML
const container = document.createElement('div');
container.style.cssText = 'max-width: 900px; margin: 0 auto; padding: 40px 20px; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; line-height: 1.6; color: #333;';

function parseMarkdown(text) {
  return text
    .replace(/^# (.*$)/gim, '<h1 style="font-size: 2.5em; margin: 0.5em 0; color: #2563eb;">$1</h1>')
    .replace(/^## (.*$)/gim, '<h2 style="font-size: 1.8em; margin: 1em 0 0.5em; color: #1d4ed8; border-bottom: 2px solid #e5e7eb; padding-bottom: 0.3em;">$1</h2>')
    .replace(/^### (.*$)/gim, '<h3 style="font-size: 1.4em; margin: 0.8em 0 0.4em; color: #374151;">$1</h3>')
    .replace(/\*\*(.+?)\*\*/g, '<strong>$1</strong>')
    .replace(/^---$/gim, '<hr style="border: none; border-top: 1px solid #e5e7eb; margin: 2em 0;">')
    .replace(/^- (.*$)/gim, '<li style="margin: 0.5em 0;">$1</li>')
    .replace(/✅/g, '<span style="color: #10b981;">✅</span>')
    .replace(/🚀/g, '<span style="font-size: 1.2em;">🚀</span>')
    .replace(/`([^`]+)`/g, '<code style="background: #f3f4f6; padding: 2px 6px; border-radius: 3px; font-family: monospace; font-size: 0.9em;">$1</code>')
    .replace(/```bash\n([\s\S]*?)```/g, '<pre style="background: #1f2937; color: #f9fafb; padding: 16px; border-radius: 8px; overflow-x: auto;"><code>$1</code></pre>')
    .replace(/```javascript\n([\s\S]*?)```/g, '<pre style="background: #1f2937; color: #f9fafb; padding: 16px; border-radius: 8px; overflow-x: auto;"><code>$1</code></pre>')
    .replace(/```\n([\s\S]*?)```/g, '<pre style="background: #f3f4f6; padding: 16px; border-radius: 8px; overflow-x: auto; border: 1px solid #e5e7eb;"><code>$1</code></pre>')
    .replace(/\[([^\]]+)\]\(([^)]+)\)/g, '<a href="$2" style="color: #2563eb; text-decoration: none; border-bottom: 1px solid #93c5fd;" target="_blank">$1</a>')
    .replace(/\n\n/g, '</p><p style="margin: 1em 0;">');
}

container.innerHTML = '<div style="background: #fff; padding: 40px; border-radius: 12px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">' + 
  '<p style="margin: 1em 0;">' + parseMarkdown(README_CONTENT) + '</p>' +
  '</div>';

document.body.innerHTML = '';
document.body.appendChild(container);
document.body.style.cssText = 'margin: 0; padding: 0; background: #f9fafb;';
document.title = 'Locanect - README';
