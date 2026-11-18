# GenZee Tech (Pvt) Ltd - Official Website & Academy Portal

A modern, fast, accessible, and SEO-optimized multi-page website for **GenZee Tech (Pvt) Ltd**, a Colombo-based technology company offering web development, full-stack systems, mobile applications, branding & graphic design, enterprise **Cyber Security Solutions**, and **GenZee Tech Academy** for school students (Grade 1 to 11).

Built with **Next.js 14 (App Router)**, **TypeScript**, **Tailwind CSS**, and **Framer Motion**.

---

## 🚀 Key Features & Highlights

- **Complete Brand Design System**: Extracted brand palette (Royal Electric Blue `#0062FF`, Vivid Cyan `#00B4FD`, Midnight Navy `#010A29`) with automatic light and dark mode toggling.
- **Dynamic Brand Configuration**: All contact information, founder quotes, social channels, stats, services, portfolios, blog posts, and academy curriculum live centrally in `/src/config/site.ts`.
- **Cyber Security Solutions Page (`/cyber-security`)**: Comprehensive ethical hacking, vulnerability scanning, penetration testing, server hardening, 24/7 security monitoring, and incident response showcase.
- **GenZee Tech Academy (`/academy`, `/academy/courses`, `/academy/enroll`)**:
  - Curriculum tracks for **Grade 1-5 (Junior Explorers)**, **Grade 6-8 (Digital Creators)**, and **Grade 9-11 (Future Innovators / O/L ICT)**.
  - Safe, child-friendly parent enrollment form with **Zod validation**, parent consent enforcement, and privacy protection.
- **Full Set of Production Pages**:
  - `Home` (`/`)
  - `About Us` (`/about`)
  - `Services Overview` (`/services`)
  - `Website Development` (`/services/web-development`)
  - `Full-Stack Development` (`/services/full-stack-development`)
  - `Mobile Applications` (`/services/mobile-applications`)
  - `Branding & Graphic Design` (`/services/branding-design`)
  - `Cyber Security Solutions` (`/cyber-security`)
  - `GenZee Tech Academy` (`/academy`)
  - `Academy Courses by Grade` (`/academy/courses`)
  - `Academy Parent Enrollment` (`/academy/enroll`)
  - `Portfolio & Case Studies` (`/portfolio`)
  - `Careers & Jobs` (`/careers`)
  - `Blog & Insights` (`/blog`) + Individual Posts (`/blog/[slug]`)
  - `Contact Us` (`/contact-us`)
  - `FAQ` (`/faq`)
  - `Privacy Policy` (`/privacy-policy`)
  - `Terms & Conditions` (`/terms-and-conditions`)
- **Full SEO & Social OpenGraph**: Dynamic XML sitemaps, `robots.txt`, JSON-LD structured data (`Organization`, `LocalBusiness`, `EducationalOrganization`), and OpenGraph social cards.
- **Floating WhatsApp Button** and interactive `<SocialLinks />` with hover animations.

---

## 🛠️ Getting Started (Local Development)

### 1. Prerequisites
- **Node.js**: v18.17+ or v20+ or v22+
- **npm** or **pnpm**

### 2. Installation
```bash
# Clone or navigate to the repository
cd "GenZee - Antigravity"

# Install dependencies
npm install
```

### 3. Environment Variables
Copy `.env.example` to `.env.local`:
```bash
cp .env.example .env.local
```
Configure your email settings:
```env
NEXT_PUBLIC_SITE_URL=https://genzeetech.com
RESEND_API_KEY=your_resend_api_key
EMAIL_FROM=notifications@genzeetech.com
EMAIL_TO=info@genzeetech.com
```

### 4. Running the Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### 5. Building for Production
```bash
npm run build
npm run start
```

---

## ⚙️ How to Edit `/src/config/site.ts`

All core data and content can be updated in a single file without modifying component code:

1. **Company & Contact Information**:
   - `siteConfig.name`, `siteConfig.tagline`, `siteConfig.contact.whatsappUrl`, `siteConfig.contact.email`, `siteConfig.contact.address`.
2. **Founder Quote & Bio**:
   - `siteConfig.founder.name`, `siteConfig.founder.title`, `siteConfig.founder.quote`, `siteConfig.founder.bio`.
3. **Social Media Links**:
   - Update `siteConfig.social.linkedin`, `facebook`, `twitter`, `youtube`, `instagram`, `tiktok`, `github`.
4. **Stats & Metrics**:
   - Update `siteConfig.stats` array to alter years of experience, projects delivered, satisfaction %, or student counts.
5. **Services, Academy Courses & Projects**:
   - Update `siteConfig.services`, `siteConfig.securityServices`, `siteConfig.academyPrograms`, and `siteConfig.projects`.

---

## ☁️ Deploying to Vercel

The website is optimized for one-click deployment on **Vercel**:

1. Push your repository to **GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial production release of GenZee Tech website"
   git remote add origin https://github.com/your-username/genzee-tech.git
   git push -u origin main
   ```
2. Log in to [Vercel](https://vercel.com) and click **"Add New Project"**.
3. Import your GitHub repository.
4. Set the Framework Preset to **Next.js**.
5. Add your Environment Variables (`NEXT_PUBLIC_SITE_URL`, `RESEND_API_KEY`, etc.).
6. Click **Deploy**. Vercel will build and serve your global edge-cached site with automated SSL.

---

## 📄 License & Attribution

© 2026 GenZee Tech (Pvt) Ltd. All rights reserved.
Developed with care in Colombo, Sri Lanka.
