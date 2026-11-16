# ImpactHub — Modern NGO Operations, Fundraising & Impact Platform

ImpactHub is a modern SaaS platform designed for non-profit organizations (NGOs) to centralize their donor relationships, fundraising appeals, beneficiary tracking, project portfolios, expense ledgers, volunteers, and verified impact analytics in one unified workspace.

Built strictly according to the specifications in **`ImpactHub_NGO_PRD.txt`**.

---

## 🚀 Key Modules & Capabilities

### 1. Executive Operations Dashboard
- **Live KPI Strip:** Total Funds Raised (₹12.8L+), Funds Raised This Month, Active Campaigns, Total Donors, Beneficiaries Helped, Active Field Projects.
- **Trajectory Visualizations:** Interactive Area Chart with multi-range filters (7D, 30D, 3M, 6M, 1Y).
- **Inflow vs Outflow:** Bar Chart contrasting incoming donations/grants against monthly program burn.
- **Spending Allocation:** Interactive Donut breakdown illustrating 87.4% direct program efficiency.
- **Operational Alerts & Tasks:** Deadline reminders, pending expense vouchers, and beneficiary follow-up notices.

### 2. Fundraising & Campaign Management
- **Campaign Directory:** Filterable by status (*Active, Draft, Completed, Paused*) and cause (*Education, Healthcare, Hunger Relief, Disaster Relief, Women Empowerment*).
- **View Toggle:** Switch seamlessly between rich visual cards and a dense operational table.
- **Multi-Step Campaign Creator:** 5-step wizard with real-time validation:
  1. *Basics* (Title, Category, Summary, Full Story)
  2. *Goal & Dates* (Target INR, Timeline, Target Beneficiary count)
  3. *Location & Impact* (Settlement location, Problem statement, Expected outcomes)
  4. *Media* (Humanitarian cover photo gallery with preset selectors & video link)
  5. *Review & Launch* (Live social card preview, Draft saving, and Confetti launch celebration)
- **Internal Campaign Management:** Live progress bar, updates feed (*with modal to post new field milestones*), audited donation transactions, and shareable public links.

### 3. Public Giving Landing Page (`/campaigns/:id/public`)
- **Emotionally Compelling Donor Experience:** Clean, standalone public-facing donor page with zero admin dashboard clutter.
- **Impact Tiers:**
  - ₹500 → Provides 1 student complete school kit & books
  - ₹1,000 → Feeds a family of 4 with emergency rations for 30 days
  - ₹2,500 → Covers mobile clinic health screening & prescription medicine for 5 villagers
  - ₹5,000 → Sponsors 1 woman with professional tailoring equipment & certification
- **Interactive Mock Donation Flow:** Real-time checkout modal supporting UPI, Credit Card, and NetBanking, instant confetti trigger, and immediate update to internal campaign raised totals and financial ledgers!
- **Supporter Wall:** Live stream of heartfelt donor messages and contributions.
- **Governance Badges:** Section 80G tax deduction certificates, FCRA compliance, and 12A trust indicators.

### 4. Donor Relationship Management (CRM)
- **Donor Roster:** Search by name, email, phone, city, or cause.
- **Segmentation:** Filter by Active, VIP (Corporate CSR), or Lapsed status, plus Recurring monthly giving badges.
- **Donor Profile Drawer:** Comprehensive sliding profile showing lifetime giving, historical donation transactions, contact details, and stewardship notes.
- **Add Donor Modal:** Register corporate CSR partners or individual patrons with form validation.

### 5. Beneficiary Case Management & Privacy Protection
- **Direct Aid Tracking:** Monitor assistance delivery across education, healthcare, and nutrition programs.
- **Case Statuses:** Active, Pending, Completed, Follow-up Required.
- **Strict Privacy Guardrail:** In accordance with the PRD, sensitive personal information is shielded with an interactive **Privacy Mask (PII protection)** to ensure vulnerable individuals are never exposed on public pages.
- **Beneficiary Profile Drawer:** Case timeline, next follow-up alerts, casework notes, and verified audit documentation counter.

### 6. Projects & Field Programs Portfolio
- **Program Overview:** Budget utilization gauges, disbursed funds, and remaining balances.
- **Interactive Milestones:** Milestone checklist with clickable checkmarks to toggle deliverables in real-time.
- **Project Lead Attribution:** Direct officer assignment and field cluster mapping.

### 7. Financial Ledger & Expense Operations
- **Audited Ledger:** Filterable transactions by Income (Donations, Grants, Sponsorships) and Expenses (Program Materials, Rations, Medical Supplies, Operations, Salaries).
- **One-Click CSV Export:** Export current filtered transactions to standard CSV for spreadsheet accounting.
- **Add Transaction Modal:** Post new income inflows or expense vouchers with project linking.

### 8. Volunteers & Field Team Directory
- **Field Force Registry:** Track active mentors, doctors, logistics leads, and compliance advisors.
- **Skill Badging:** Tag volunteers with specializations (STEM Education, General Medicine, Translation, etc.).
- **Hours Log:** Verified contribution tracking (429+ logged service hours).

### 9. Impact & Executive Reports
- **Multi-Category Reports:** Monthly Impact Report, Fundraising Performance, Financial Summary, Project Performance, and Donor Retention.
- **Printable Document Canvas:** Clean letterhead format with executive narratives, KPI matrix, deliverable tables, and digital trustee sign-off.
- **Export Modal:** Download high-resolution PDF or raw CSV data packages.

### 10. Organization Settings & Role-Based Access Control
- **Entity Profile:** Manage legal name, 80G certificate numbers, registered address, and official contacts.
- **Staff Access:** Invite colleagues with specific roles (*Admin, Finance Manager, Fundraising Manager, Program Manager, Volunteer Manager, Viewer*).
- **RBAC Matrix:** Visual permission grid detailing module privileges.
- **Demo Controls:** One-click reset to Hope Foundation default seed data.

---

## 🛠️ Architecture & Tech Stack

- **Framework:** React 18 with TypeScript
- **Bundler:** Vite 5 with code splitting and manual chunking
- **Styling:** Tailwind CSS with custom design system (Deep Navy, Slate, Impact Teal, Emerald)
- **Icons:** Lucide React
- **Data Visualizations:** Recharts (Area charts, Bar charts, Donut breakdown)
- **Routing:** React Router v6 with nested layout shell and standalone public routes
- **State Layer:** Reactive `ImpactService` with event subscription pattern and persistent `localStorage` synchronization
- **Delight:** Canvas Confetti for celebratory campaign launches and donations

---

## 📦 Getting Started

### Install Dependencies
```bash
npm install
```

### Run Local Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### Build for Production
```bash
npm run build
```
Creates an optimized, minified bundle in the `dist/` directory.

### Preview Production Build
```bash
npm run preview
```

---

## 🌟 Demo Data Benchmark (Hope Foundation)
- **Total Funds Raised:** ₹12.8L+
- **Donors on File:** 11+ detailed profiles (Corporate CSR & Patrons)
- **Beneficiaries:** 3,842+ assisted
- **Active Campaigns:** 4 running appeals, 1 draft, 1 completed
- **Direct Programs:** 4 active field interventions across Karnataka and Delhi NCR
