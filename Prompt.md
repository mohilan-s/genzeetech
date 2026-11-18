Build a modern, responsive, multi-page website for "GenZee Tech (Pvt) Ltd",
a software and technology company based in Colombo, Sri Lanka. The company
offers web development, full-stack development, mobile apps, branding & design,
CYBER SECURITY SOLUTIONS, and runs "GenZee Tech Academy", an IT skill
development academy for school students (Grade 1 to 11).
Use Next.js (App Router) + TypeScript + Tailwind CSS + Framer Motion.
Make it production-ready, fast, accessible and SEO-optimised.

=== BRAND CONFIG (create /config/site.ts and use it everywhere) ===
- Company name: GenZee Tech (Pvt) Ltd (short name: GenZee Tech)
- Tagline: "We Build Digital Experiences"
- Logo: /public/Logo.png (provided; use in navbar, footer, favicon and Open
  Graph image via next/image, keep aspect ratio; make it look good on both
  light and dark backgrounds, e.g. a white pill behind it in dark mode if
  needed).
- Founder photo: /public/Mohilan.jpg (provided)
- WhatsApp: +94 779669761
  Link: https://wa.me/94779669761?text=Hi%20GenZee%20Tech%2C%20I%27m%20interested%20in%20starting%20a%20new%20project.
- Email: info@genzeetech.com
- Address: Colombo, Sri Lanka
- Social links (demo URLs, editable in one place):
  LinkedIn: https://www.linkedin.com/company/genzeetech
  Facebook: https://www.facebook.com/genzeetech
  X (Twitter): https://x.com/genzeetech
  YouTube: https://www.youtube.com/@genzeetech
  Instagram: https://www.instagram.com/genzeetech
  TikTok: https://www.tiktok.com/@genzeetech
  WhatsApp: (use the WhatsApp link above)
  GitHub: https://github.com/genzeetech
- Copyright: "© 2026 GenZee Tech (Pvt) Ltd. All rights reserved."

Extract 2 to 3 accent colours from Logo.png and use them as the palette
(primary, secondary, accent) so the whole site matches the brand.

=== SOCIAL MEDIA ICONS ===
Create a reusable <SocialLinks /> component showing icon buttons for LinkedIn,
Facebook, X, YouTube, Instagram, TikTok, WhatsApp and GitHub (use lucide-react
or react-icons / Simple Icons). Round buttons, brand-colour hover effect,
open in a new tab with rel="noopener noreferrer", aria-labels on each. Use it
in the footer, the Contact page, the Founder section, and the Academy page.
All URLs come from /config/site.ts so I can swap in real links later.

=== PAGES ===
1. Home
2. About Us (company story, mission/vision, values, Founder section, team)
3. Services (overview of all 6 services)
4. Web Development
5. Full-Stack Development
6. Mobile Applications
7. Branding & Graphic Design
8. Cyber Security Solutions (NEW)
9. GenZee Tech Academy (NEW) with sub-pages: /academy/courses, /academy/enroll
10. Portfolio
11. Careers
12. Blog (list + single post)
13. Contact Us
14. Privacy Policy  15. Terms & Conditions  16. FAQ

=== NAVBAR ===
Sticky navbar with Logo.png and links: Home, About Us, Services (dropdown with
all 6 services + one-line descriptions: Web Development, Full-Stack
Development, Mobile Applications, Branding & Design, Cyber Security),
Academy (highlighted, links to /academy), Portfolio, Careers, More (Blog, FAQ).
Right side: dark/light toggle and a "Let's Talk!" CTA button to /contact-us.
Mobile hamburger menu. Navbar gets a blur and shadow after scrolling.

=== HOME PAGE SECTIONS (in this order) ===
1. Hero: small "Available for new projects" badge, big headline
   "We Build Digital [Experiences | Products | Platforms | Solutions]" with an
   animated rotating last word, subtext "Websites, apps, cyber security and
   digital experiences built to help businesses grow.", two buttons
   ("Start a project" opens the WhatsApp link, "View work" goes to /portfolio),
   and a 5-star line "4.8/5 · 300+ clients". Rounded (20px) full-width hero
   card with a soft gradient background and subtle floating shapes.
2. Stats strip: animated count-up numbers on scroll (Years of Experience,
   Projects Delivered, Client Satisfaction %, Happy Clients). Editable in config.
3. Client logos: infinite marquee of placeholder logos.
4. Services: two rows of 3 cards, each with a number, title, description,
   tech tags and "View service" link:
   - 01 Website Development (WordPress, Elementor, React)
   - 02 Full-Stack Development (Next.js, Node.js, Supabase)
   - 03 Mobile Applications (React Native, API, Cloud)
   - 01 Brand Identity (Identity, Logo, Guidelines)
   - 02 Graphic Design (Photoshop, Illustrator, InDesign)
   - 03 Cyber Security (Pen Testing, Audits, Monitoring)
   Add a visible "UI/UX Design" mention within Branding & Design.
5. CYBER SECURITY highlight band (dark section): headline "Protect What You've
   Built.", 4 mini feature cards (Vulnerability Assessment, Penetration
   Testing, Security Monitoring, Incident Response), subtle animated
   shield/lock/scan-line visual, and a "Get a free security consultation" button.
6. GENZEE TECH ACADEMY highlight band (bright, friendly colours): headline
   "Where Young Minds Learn Technology.", subtext "Basic IT skills and
   technology knowledge for students from Grade 1 to Grade 11.", 3 grade-group
   cards (Grade 1-5, Grade 6-8, Grade 9-11), a "Explore the Academy" button and
   an "Enroll Now" button. Use playful but professional icons and illustrations.
7. How we work: 3 steps (Discover, Design & Build, Launch & Grow) with small
   animated mock UI visuals.
8. Portfolio showcase: 5 featured project cards (country flag, project name,
   category, title, short description, placeholder image, "Visit Website"
   button). Use clearly fictional placeholder projects.
9. Tools marquee: Figma, Framer, WordPress, Elementor, React, Next.js,
   JavaScript, TypeScript, Node.js, Supabase, Vercel, GitHub
   (icons from https://cdn.simpleicons.org/<name>).
10. "Why GenZee Tech" bento grid with 4 features: One Connected Team, Proven
    Experience, Global Delivery, Beyond Launch (support, security monitored,
    performance optimised), each with a small animated visual.
11. FOUNDER section: large rounded photo from /public/Mohilan.jpg
    (next/image, object-cover, soft shadow, subtle decorative shape behind it),
    name "S. Mohilan", title "Founder & CEO", company "GenZee Tech (Pvt) Ltd",
    a short placeholder bio / vision quote (3 to 4 lines, clearly editable), and
    the <SocialLinks /> component. Two-column layout on desktop, stacked on
    mobile. Also reuse this section on the About Us page.
12. Testimonials: Google-style review carousel with rating badge, avatar
    initial, name, role, "x months ago". Placeholder reviews.
13. Latest blog posts: 3 cards from local MDX files.
14. Final CTA banner: "Ready to Build Something Great?" with "Work With Us"
    (/contact-us) and "Explore our work" (/portfolio).
15. Footer: Logo.png, short description, <SocialLinks />, columns for
    Company (About, Portfolio, Careers, Contact), Services (all 6), Academy
    (Courses, Enroll), Legal (Privacy, Terms, FAQ), plus email, address and
    copyright.

=== CYBER SECURITY SOLUTIONS PAGE (/cyber-security) ===
Same visual style as the other service pages. Sections:
- Hero: "Cyber Security Solutions" + short description + CTA "Get a Free
  Security Consultation" (WhatsApp) with an animated shield/scan visual.
- Services grid: Vulnerability Assessment, Penetration Testing (Web, Mobile,
  Network), Website & Server Hardening, Security Audits & Compliance Review,
  24/7 Security Monitoring, Incident Response & Recovery, Malware Removal,
  Cloud & Network Security, Staff Security Awareness Training, Backup &
  Disaster Recovery.
- "Our Security Process" timeline: Assess → Protect → Monitor → Respond.
- Who we protect: Small Businesses, Startups, E-commerce, Schools, Enterprises.
- Tools/standards badges (text only, no logos): OWASP, ISO 27001-aligned,
  Firewalls, SSL/TLS, Encryption.
- FAQ accordion about security services.
- CTA banner and contact form variant (service pre-selected as Cyber Security).

=== GENZEE TECH ACADEMY PAGE (/academy) ===
Brighter, friendlier colour treatment, but same fonts, spacing and component
style as the rest of the site. Sections:
- Hero: "GenZee Tech Academy", subtext "Building the next generation of
  tech-smart students, Grade 1 to Grade 11.", buttons "Enroll Now" and
  "View Courses", with a playful animated illustration.
- Programs by level (tabs or cards):
  - Grade 1-5 (Junior Explorers): computer basics, typing, safe internet use,
    Paint/drawing tools, intro to logical thinking, block-based coding
    (Scratch).
  - Grade 6-8 (Digital Creators): MS Office (Word, Excel, PowerPoint),
    internet research skills, Canva & basic graphic design, intro to
    programming (Scratch/Python basics), basic web pages (HTML/CSS).
  - Grade 9-11 (Future Innovators): programming (Python/JavaScript),
    web development, ICT exam support (O/L preparation), database basics,
    intro to cyber security & online safety, robotics/AI awareness, mini
    projects and portfolio building.
- Why choose the Academy: qualified instructors, small batches, hands-on
  projects, child-friendly curriculum, safe online environment, certificates,
  progress reports to parents.
- Learning journey: Learn → Practice → Build → Certificate.
- Class formats: Weekday / Weekend batches, In-person / Online (editable
  placeholders).
- Student projects gallery (placeholder cards).
- Parent testimonials (placeholders).
- Fees & schedule: placeholder cards with "Contact us for details".
- FAQ accordion (age groups, laptop required?, batch size, certificates, etc.).
- Enrollment page (/academy/enroll): a form meant to be filled out by a
  PARENT/GUARDIAN (parent name, phone, email, student first name, grade,
  preferred batch, message) with validation (react-hook-form + zod).
  Add a consent checkbox and a note that data is used only for enrollment.
  Collect the minimum student data needed. No student photos or personal
  details are displayed publicly on the site.
- /academy/courses: course listing with filters by grade group.

=== OTHER PAGES ===
- About Us: company story, mission, vision, values, Founder section
  (reused), small team grid with placeholders, timeline.
- Services overview: 6 service cards linking to detail pages.
- Web Dev, Full-Stack, Mobile, Branding pages: hero, what's included,
  process, tech stack, related projects, CTA.
- Portfolio: category filters (Web, Mobile, Branding, Full-Stack, Security).
- Careers: open roles from a JSON file with "Apply via email" buttons.
- Blog: MDX posts, categories, reading time, 3 sample posts (include one on
  cyber security and one on kids learning to code).
- FAQ: accessible accordion.
- Privacy Policy and Terms: sensible placeholder legal text, including a
  section on children's data for the Academy.
- Contact: form (name, email, phone, service dropdown including
  "Cyber Security" and "Academy Enquiry", message) with react-hook-form + zod.
  POST to /api/contact which emails info@genzeetech.com via Resend or
  Nodemailer using .env variables (provide .env.example). Show address,
  email, WhatsApp button, <SocialLinks />, and an embedded map of Colombo.
- Floating WhatsApp button on every page (bottom-right).

=== DESIGN SYSTEM ===
- Clean, premium, lots of whitespace, rounded corners (16 to 24px), soft shadows.
- Colour tokens as CSS variables with light and dark themes (auto via
  prefers-color-scheme plus a manual toggle).
- One distinctive display font and one clean body font via next/font. Avoid
  generic default styling.
- Subtle scroll-reveal animations, card hover lifts, smooth marquees. Respect
  prefers-reduced-motion.
- Mobile-first, fully responsive, accessible (semantic HTML, alt text, focus
  states, WCAG AA contrast). Founder photo alt text: "S. Mohilan, Founder & CEO
  of GenZee Tech".

=== SEO & PERFORMANCE ===
- Per-page metadata, Open Graph + Twitter cards, canonical URLs, sitemap.xml,
  robots.txt, favicon generated from Logo.png.
- JSON-LD: Organization (with founder S. Mohilan and sameAs social links),
  LocalBusiness (Colombo, Sri Lanka), EducationalOrganization (Academy),
  BlogPosting.
- next/image with AVIF/WebP, lazy loading, minimal client JS, target
  Lighthouse 90+.

=== DELIVERABLES ===
- Clean folder structure with reusable components: Navbar, Hero, StatCounter,
  Marquee, ServiceCard, ProjectCard, HowWeWork, WhyUs, SecurityBand,
  AcademyBand, FounderSection, SocialLinks, TestimonialCarousel, BlogCard,
  CTA, Footer, WhatsAppButton, ContactForm, EnrollForm.
- README with setup steps, env variables, how to edit /config/site.ts, and
  Vercel deployment steps.
- When finished: run the dev server, open every page at mobile (375px) and
  desktop (1440px), confirm Logo.png and Mohilan.jpg load correctly, and fix
  any layout issues, broken links or console errors.

Start with a short build plan, then build the Home page first, confirm it
looks right, then build the remaining pages one group at a time
(services, Cyber Security, Academy, then the rest).