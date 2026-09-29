# Modern Personal Portfolio Website

A sleek, responsive, and high-performance personal portfolio website built with **React**, **Vite**, and **Tailwind CSS**. Designed specifically for a B.Tech student passionate about Artificial Intelligence, modern web development, and digital productivity.

---

## 🚀 Key Features

- **Theme Toggle**: Seamless dark mode and light mode switching with persistence in `localStorage`.
- **High-Impact Hero Section**: Status badge (*"Open to Internships"*), dynamic gradient text, interactive tech showcase card, and quick stats.
- **Student-Friendly About Section**: Narrative introduction, core specialization cards, and resume download/preview.
- **Academic Timeline**: B.Tech coursework tags, relevant learning areas, and academic highlights.
- **Filterable Skills Grid**: 8 core areas (HTML, CSS, JavaScript, Python, Artificial Intelligence, Generative AI, Web Development, Digital Productivity) with proficiency meters and category tabs.
- **Projects Showcase**: Detailed project cards with technology pills, live demo links, GitHub repo buttons, and an interactive full-detail modal.
- **Milestones & Achievements**: Certifications, Hackathons, Courses, and Awards with an expandable slot for adding new credentials.
- **Interactive Contact Section**: Direct contact cards (Email with 1-click copy to clipboard, LinkedIn, GitHub, Location) + validated contact form with toast confirmation.
- **Modern Micro-interactions**: Smooth scrolling with scroll spy nav highlighting, top scroll progress bar, hover glow effects, and responsive mobile drawer menu.

---

## 📁 Project Structure

```
portfolio-website/
├── index.html                 # HTML5 entry configured with Plus Jakarta Sans & Tailwind
├── package.json               # Vite, React, and Tailwind dependencies
├── vite.config.js             # Vite configuration
├── tailwind.config.js         # Tailwind theme & color definitions
├── postcss.config.js          # PostCSS configuration
├── vercel.json                # Vercel SPA routing configuration
├── README.md                  # Project documentation & deployment guide
├── public/
│   └── favicon.svg            # Custom modern SVG favicon
└── src/
    ├── main.jsx               # React DOM entry
    ├── App.jsx                # Layout orchestrator, theme manager, scroll spy, toast
    ├── index.css              # Custom utilities, animations, scrollbars
    ├── data/
    │   └── portfolioData.js   # Central configuration file for all personal data
    └── components/
        ├── Icons.jsx          # Pixel-crisp inline SVG icon components
        ├── Navbar.jsx         # Header with theme toggle & mobile drawer
        ├── Hero.jsx           # Hero with CTAs, code preview, and stats
        ├── About.jsx          # Student bio, philosophy, and focus cards
        ├── Education.jsx      # B.Tech timeline and coursework badges
        ├── Skills.jsx         # Interactive skill cards & category filter
        ├── Projects.jsx       # Featured projects & details modal
        ├── Achievements.jsx   # Tabbed achievements & certifications
        ├── Contact.jsx        # Direct info, copy email, and contact form
        └── Footer.jsx         # Footer with quick links & back-to-top button
```

---

## 🛠️ How to Customize Your Information

All content on the portfolio is centralized in:
`src/data/portfolioData.js`

You can easily update:
1. **Personal Information**:
   - `name`: Change to your name
   - `college`: Your college/university name
   - `location`: Your city and country (e.g. "New Delhi, India")
   - `email`: Your personal or university email
   - `linkedin`: Your LinkedIn profile URL
   - `github`: Your GitHub profile URL
   - `resumeUrl`: Link to your PDF resume or Google Drive link
2. **Projects**: Add, modify, or remove projects in `projectsData`.
3. **Skills**: Adjust proficiency percentages and descriptions in `skillsData`.
4. **Achievements**: Add your hackathon certificates, awards, and course completions in `achievementsData`.

---

## 💻 Running the Website Locally

### Option 1: Instant Local Server (Zero-Dependency)
From the `portfolio-website` directory, run:
```bash
python3 -m http.server 5173
```
Then open your browser and navigate to:
[http://localhost:5173](http://localhost:5173)

### Option 2: Vite Dev Server (Requires Node.js & npm)
If Node.js is installed on your machine:
```bash
# 1. Install dependencies
npm install

# 2. Start Vite local server
npm run dev
```

---

## 🌐 Deploying to Vercel

This repository is pre-configured with `vercel.json` for seamless deployment.

### Method 1: Deploy via GitHub (Recommended)
1. Push this folder to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit of modern student portfolio"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
2. Log into [Vercel](https://vercel.com).
3. Click **"Add New Project"** and import your GitHub repository.
4. Vercel will automatically detect Vite and configure the build command (`npm run build`) and output directory (`dist`).
5. Click **"Deploy"**!

### Method 2: Deploy via Vercel CLI
```bash
npm install -g vercel
vercel
```

---

## 🎨 Design System & Technologies
- **Framework**: React 18
- **Styling**: Tailwind CSS with custom `brand` palette and dark mode
- **Typography**: Plus Jakarta Sans & Inter
- **Icons**: Custom SVG icons with Lucide design language
- **Deployment**: Vercel ready
