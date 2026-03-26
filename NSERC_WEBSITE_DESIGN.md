# NSERC Premium Mobile‑First Website Design Brief

## 1) Context and goals
Niger State Electricity Regulatory Commission (NSERC) needs a modern, trusted public platform that balances:
- public service delivery (complaints, forms, guidance),
- regulatory transparency (instruments, orders, notices, consultation drafts),
- institutional credibility (clean government-grade design with premium UX), and
- operational efficiency (admin-managed content and document workflows).

Primary audiences:
- Electricity customers and community stakeholders,
- licensees and market participants,
- policymakers, media, and civil society,
- internal NSERC teams and administrators.

Core outcomes:
1. **Fast complaint submission and tracking** with clear SLAs and status updates.
2. **Easy access to public documents** (regulatory instruments, forms, directives, consultation papers).
3. **Strong trust signals** (commission profile, legal basis, governance, performance reports).
4. **Content agility** so admins can update pages, hero banners, media, and documents without developers.

---

## 2) Brand direction from provided logo
Observed logo cues:
- Dominant green palette and official seal geometry,
- Black and gold accents in the accompanying wordmark,
- Institutional tone that should feel authoritative, calm, and premium.

Suggested brand system:
- **Primary:** Deep Emerald `#0E6B3A`
- **Secondary:** Forest Green `#1C8A50`
- **Accent:** Gold `#C79A2B`
- **Text primary:** Charcoal `#1C1C1C`
- **Background:** Warm off-white `#F7F8F6`
- **Support:** Slate `#5F6B66`

Typography:
- Headings: **Manrope** / **Sora** (bold, clean, contemporary)
- Body: **Inter** / **Source Sans 3**

Visual style:
- Rounded cards (12–16px radius), soft shadows, generous spacing,
- High-contrast buttons and status chips,
- Photo style: power infrastructure, customer service touchpoints, state development.

---

## 3) Information architecture (recommended top menu + submenus)
You mentioned earlier menus: **About NSERC, Regulatory Instruments, Services, Resources, News & Media**. Below is a refined and complete structure.

### A. About NSERC
- Overview
- Legal Mandate
- Vision, Mission & Values
- Leadership / Commissioners
- Organizational Structure
- Strategic Plan
- Service Charter
- Contact & Office Locations

### B. Regulatory Instruments
- All Instruments (search/filter)
- Regulations
- Orders & Directives
- Guidelines & Codes
- Consultation Papers (Drafts)
- Licensing Framework
- Tariff Methodologies / Decisions
- Compliance Notices

### C. Services
- Lodge a Complaint
- Track Complaint Status
- Customer Protection Desk
- License/Permit Applications (if in scope)
- Stakeholder Consultations (submissions)
- Requests for Clarification / Interpretation

### D. Resources
- Forms & Templates
- Downloads Center
- FAQ
- Consumer Education
- Market Data & Reports
- Procurement / Tenders (optional)
- Career Opportunities (optional)

### E. News & Media
- Press Releases
- News Updates
- Events & Public Hearings
- Photo Gallery
- Video Briefings
- Public Notices

Utility navigation (always visible):
- **Emergency contacts**
- **Complaint CTA**
- **Document Search**
- Accessibility controls (text size, contrast)

---

## 4) Shared UX requirements for both design options
1. **Mobile-first architecture:** one-thumb actions, sticky CTAs, short forms.
2. **Fast findability:** persistent global search across documents + pages.
3. **Trust and transparency:** publication date, revision history, signed PDF tags.
4. **Accessibility:** WCAG-aligned color contrast, keyboard navigation, clear labels.
5. **Multilingual readiness:** English-first with architecture for future local language support.
6. **Performance:** compressed images, lazy loading, CDN-backed static assets.

---

## 5) Design Option 1: “Executive Civic” (formal premium)
A clean, high-authority government design language with strong hierarchy and restrained visuals.

### Home page layout
1. **Hero strip**
   - Short trust headline (“Transparent Electricity Regulation for Niger State”)
   - 2 primary CTAs: **Lodge Complaint** and **Browse Regulatory Instruments**
   - Rotating verified announcements.

2. **Quick service tiles (4–6)**
   - Lodge Complaint
   - Track Complaint
   - Download Forms
   - View Latest Orders
   - Consultation Submissions

3. **Regulatory spotlight**
   - Latest 3 instruments with tags: Regulation / Order / Guideline
   - “What changed” mini-summary line.

4. **Consumer protection panel**
   - Rights and obligations snapshot
   - Escalation steps visual timeline.

5. **News + hearings**
   - Combined stream with filters for media vs notices.

6. **Footer megablock**
   - legal links, anti-corruption notice, FOI/contact details, social channels.

### UI character
- Spacious and elegant,
- Fewer animations, high readability,
- Gold accents used sparingly for premium feel.

### Best when
- You want credibility and policy seriousness to be the dominant impression.

---

## 6) Design Option 2: “Stakeholder Service Hub” (dynamic premium)
A more interactive and service-oriented experience focused on tasks and stakeholder journeys.

### Home page layout
1. **Action-first hero**
   - Greeting + search bar (“Search instruments, forms, notices…”)
   - Prominent segmented actions: **Complain | Download | Learn | Engage**

2. **Journey blocks by audience**
   - Consumers
   - Licensees
   - Investors/Developers
   - Media/Civil Society
   Each block reveals top tasks.

3. **Complaint journey tracker preview**
   - Step 1 Submit → Step 2 Review → Step 3 Investigation → Step 4 Resolution
   - Link to status page.

4. **Intelligent document center**
   - Filter chips: Type, Year, Topic, Status (Draft/Active/Archived)
   - “Most downloaded” and “recently updated”.

5. **Data & insights panel**
   - Complaint resolution metrics
   - Instruments published this quarter
   - Hearing schedule snapshot.

### UI character
- More components, dynamic chips, status indicators,
- Slightly richer interaction and animations,
- Still official, but more “digital-service” feeling.

### Best when
- You want strong public engagement and repeat task completion.

---

## 7) Functional modules (front-end + partial backend)

### 7.1 Complaint management module
Public features:
- Complaint intake form with categories (billing, metering, outage quality, disconnection, service failure).
- Required fields + evidence upload (images/docs).
- Consent + privacy statement.
- Unique complaint ID issued instantly.
- Status tracking page with timeline and timestamps.

Admin features:
- Queue dashboard by status and SLA due date,
- Assign officers, add internal notes,
- Request additional information,
- Escalation workflow,
- Resolution issuance with downloadable outcome letter.

### 7.2 Regulatory instruments engine
Public features:
- Filterable repository (type, year, topic, status),
- Full-text search and metadata tags,
- Version history, effective date, and repeal/supersede relation,
- Download analytics (non-personal).

Admin features:
- Draft → Review → Publish workflow,
- Rich metadata editor,
- Bulk upload and archive,
- “Related instruments” linking,
- Scheduled publication.

### 7.3 CMS/content administration
- Update homepage banners, images, and write-ups,
- Manage menus and featured links,
- Publish news, notices, events,
- Role-based access (Super Admin, Content Editor, Complaint Officer, Legal Reviewer),
- Audit log for changes.

---

## 8) Recommended page inventory (MVP)
1. Home
2. About pages (overview, mandate, leadership)
3. Instruments listing + detail page
4. Complaint submit page
5. Complaint status page
6. Forms/downloads page
7. News listing + article page
8. Contact page
9. FAQ
10. 404 + maintenance page

---

## 9) Data model essentials (high level)
- **User** (admin roles only initially)
- **Complaint** (id, complainant details, category, narrative, attachments, status, SLA, assigned officer)
- **ComplaintUpdate** (status transitions, timestamps, notes)
- **Instrument** (title, type, reference no., issue date, effective date, status, version, file)
- **DocumentAsset** (forms, templates, reports)
- **NewsPost/Event**
- **MediaAsset**
- **AuditLog**

---

## 10) Security, governance, and compliance checklist
- HTTPS everywhere + secure file upload scanning,
- Role-based permissions and least privilege,
- Full audit trail for complaint and instrument edits,
- Data retention policy for personal complaint records,
- Anti-spam and bot protection on public forms,
- Backup + disaster recovery plan,
- Privacy notice and terms of use.

---

## 11) Suggested technology architecture (pragmatic)
- **Frontend:** Next.js (mobile-first SSR/ISR for speed + SEO)
- **UI:** Tailwind + component system
- **Backend modules:**
  - Complaints API (workflow + SLA service)
  - Instruments API (metadata + document indexing)
  - CMS API (content blocks, pages, menus)
- **Storage:** object storage for PDFs/media
- **Search:** document index for fast retrieval
- **Admin auth:** secure RBAC with MFA for privileged accounts

---

## 12) Selection guidance: which option should you choose?
- Choose **Option 1 (Executive Civic)** if your first priority is institutional gravitas and policy authority.
- Choose **Option 2 (Stakeholder Service Hub)** if your first priority is task completion, engagement, and frequent public interactions.

A practical path:
- Start with Option 1 shell (credibility),
- Borrow Option 2 service widgets (complaint tracker, smart document filters),
- This hybrid gives premium image + practical usability.

---

## 13) Immediate next deliverables (if you approve one option)
1. Detailed sitemap with all final submenus.
2. Mobile wireframes for 8 critical pages.
3. UI kit (colors, typography, button states, form states).
4. Complaint workflow diagram (public + internal admin).
5. Instruments lifecycle diagram (draft to archive).
6. 3-phase implementation plan (MVP, V2, optimization).

---

## 14) Option A execution package (detailed handoff for AI implementation)
You selected **Option A / Executive Civic**. The section below is a complete implementation handoff designed to reduce ambiguity.

### 14.1 Full sitemap (definitive)

#### Public routes
- `/`
  - Home (Executive Civic layout)
- `/about`
  - `/about/overview`
  - `/about/legal-mandate`
  - `/about/vision-mission-values`
  - `/about/leadership`
  - `/about/organizational-structure`
  - `/about/strategic-plan`
  - `/about/service-charter`
  - `/about/contact-locations`
- `/regulatory-instruments`
  - Listing with filters/search
  - `/regulatory-instruments/:slug` (detail)
  - `/regulatory-instruments/type/regulations`
  - `/regulatory-instruments/type/orders-directives`
  - `/regulatory-instruments/type/guidelines-codes`
  - `/regulatory-instruments/type/consultation-papers`
  - `/regulatory-instruments/type/licensing-framework`
  - `/regulatory-instruments/type/tariff-methodologies`
  - `/regulatory-instruments/type/compliance-notices`
- `/services`
  - `/services/lodge-complaint`
  - `/services/track-complaint`
  - `/services/customer-protection-desk`
  - `/services/license-permit-applications` (feature-flag if not live)
  - `/services/stakeholder-consultations`
  - `/services/clarification-requests`
- `/resources`
  - `/resources/forms-templates`
  - `/resources/download-center`
  - `/resources/faq`
  - `/resources/consumer-education`
  - `/resources/market-data-reports`
  - `/resources/procurement-tenders` (optional)
  - `/resources/careers` (optional)
- `/news-media`
  - `/news-media/press-releases`
  - `/news-media/news-updates`
  - `/news-media/events-hearings`
  - `/news-media/photo-gallery`
  - `/news-media/video-briefings`
  - `/news-media/public-notices`
  - `/news-media/:slug` (article/event detail)
- `/search`
- `/contact`
- `/privacy-policy`
- `/terms-of-use`
- `/accessibility`
- `/404`
- `/maintenance`

#### Complaint routes
- `/complaints/new`
- `/complaints/track`
- `/complaints/track/:reference`
- `/complaints/checklist` (before-submit guidance)
- `/complaints/acknowledgement/:reference`

#### Admin routes
- `/admin/login`
- `/admin/dashboard`
- `/admin/content/pages`
- `/admin/content/menus`
- `/admin/media-library`
- `/admin/news`
- `/admin/instruments`
  - create/edit/publish/archive/version history
- `/admin/documents`
- `/admin/complaints`
  - queue/assign/escalate/resolve/export
- `/admin/users-roles`
- `/admin/audit-logs`
- `/admin/settings` (branding, contact blocks, homepage sections)

### 14.2 Global navigation model
- Header (sticky):
  - Logo left
  - Main menu center (About, Regulatory Instruments, Services, Resources, News & Media)
  - Utility right: Search icon, Emergency contact chip, Lodge Complaint CTA
- Mobile header:
  - Left: logo mark
  - Right: hamburger + complaint CTA button
- Footer:
  - 4-column structure: About, Services, Resources, Legal
  - Contact block, social links, copyright, last-updated timestamp

### 14.3 Mobile wireframes section-by-section (text blueprint)

#### A) Home `/`
1. Top utility strip (Emergency line + office hours)
2. Header (logo + menu icon + complaint CTA)
3. Hero
   - Heading, 2-line subtext, primary CTA (Lodge Complaint), secondary CTA (Browse Instruments)
4. Quick actions (2x2 cards)
   - Lodge Complaint, Track Complaint, Download Forms, Latest Orders
5. Regulatory Spotlight carousel/list
   - 3 latest documents with type/date/effective status chips
6. Consumer Protection block
   - Rights summary + “How complaint resolution works” mini timeline
7. News & Hearings tabs
8. Commission message / trust block
9. Footer links + contacts

#### B) Instruments listing `/regulatory-instruments`
1. Page heading + intro
2. Search input (sticky on scroll)
3. Filter drawer (mobile bottom sheet): Type, Year, Topic, Status
4. Sort dropdown (Newest, Most downloaded, Alphabetical)
5. Results cards
   - Title, type chip, reference no, issue date, effective date, summary, download button
6. Pagination / load more
7. Empty state with clear recovery actions

#### C) Instrument detail `/regulatory-instruments/:slug`
1. Breadcrumb
2. Title, type, reference number, status badge
3. Key metadata table (issue/effective/review dates)
4. Summary (“What this instrument covers”)
5. Download/view buttons
6. Version history accordion
7. Related instruments list
8. Share/print controls

#### D) Lodge complaint `/complaints/new`
1. Intro + disclaimer + expected timelines
2. Stepper (1 Personal info, 2 Complaint details, 3 Evidence upload, 4 Review & submit)
3. Field groups:
   - Identity/contact
   - Service provider/disco
   - Complaint category/subcategory
   - Narrative with guidance prompts
4. File upload area (jpg/png/pdf, max size)
5. Consent checkbox + privacy text
6. Submit CTA (disabled until valid)
7. Success screen with complaint reference and next steps

#### E) Track complaint `/complaints/track`
1. Input: reference + email/phone verification
2. Status timeline component
3. Officer/request updates
4. Downloadable acknowledgement/resolution letters
5. Escalation guidance block

#### F) News & media list `/news-media/...`
1. Tab switcher (Press, News, Events, Notices)
2. Featured story card
3. Standard article list cards
4. Date filter + keyword search

#### G) Contact `/contact`
1. Phone/email/office cards
2. Embedded map
3. Contact form
4. Complaint redirect notice (“for dispute use complaint portal”)

#### H) Admin dashboard `/admin/dashboard`
1. KPI cards (open complaints, SLA due, published instruments, pending drafts)
2. Work queues (complaints due today, drafts awaiting review)
3. Recent activity feed (audit logs)
4. Quick actions

### 14.4 Component inventory (design system)
- Buttons: primary/secondary/ghost/destructive with loading/disabled states
- Inputs: text, textarea, select, multiselect, date, file uploader
- Data display: cards, tables, chips, timeline, badges, accordions
- Feedback: toast, inline alerts, modal confirmations, skeleton loaders
- Navigation: breadcrumb, tabs, pagination, drawer, mega menu
- Content blocks: hero, callout, stats strip, FAQ accordion, document card

### 14.5 Content model (CMS schema)
- Page (title, slug, SEO, body blocks, publish state)
- Menu (location, items, hierarchy)
- HeroBanner (headline, subtext, image/video, CTAs, schedule)
- NewsPost (category, title, excerpt, body, media, publish date)
- Instrument (type, ref no, title, summary, issue date, effective date, status, file, related)
- ResourceDocument (form/template/report class, tags, file)
- ComplaintCategory (name, subcategories, SLA rules)
- ContactInfo (addresses, phone, office hours)
- FAQItem (question, answer, topic)

### 14.6 Backend API contract (high-level)
- Auth:
  - `POST /api/auth/login`
  - `POST /api/auth/logout`
  - `GET /api/auth/me`
- Complaints:
  - `POST /api/complaints`
  - `GET /api/complaints/track?reference=...`
  - `POST /api/complaints/:id/messages`
  - `PATCH /api/admin/complaints/:id/status`
- Instruments:
  - `GET /api/instruments`
  - `GET /api/instruments/:slug`
  - `POST /api/admin/instruments`
  - `PATCH /api/admin/instruments/:id`
  - `POST /api/admin/instruments/:id/publish`
- CMS:
  - `GET /api/pages/:slug`
  - `PATCH /api/admin/pages/:id`
  - `GET /api/menus/:location`
  - `PATCH /api/admin/menus/:location`
- Media/documents:
  - `POST /api/admin/uploads`
  - `GET /api/documents`

### 14.7 Non-functional requirements
- Performance:
  - Mobile Lighthouse target >= 85 performance, >= 95 accessibility
  - Largest contentful paint < 2.5s on 4G
- Security:
  - RBAC + MFA for admins
  - Rate limiting + captcha on public complaint form
  - Anti-malware scan for uploads
  - Immutable audit logs
- Reliability:
  - Daily backups + 30-day retention
  - Uptime target 99.5%

### 14.8 One-time implementation plan (single-run build)

#### Phase 0: Foundation (Day 1–3)
- Setup monorepo/app structure
- Establish design tokens, typography, spacing scale
- Build base layout, header/footer, routing skeleton
- Configure auth/RBAC, logging, environment variables

#### Phase 1: Public experience core (Day 4–10)
- Implement Home, About, Contact, Resources, News listings
- Implement global search and document cards
- Implement responsive navigation and menu hierarchy

#### Phase 2: Regulatory instruments engine (Day 11–15)
- Create instrument schema + admin CRUD
- Implement public list/detail with filters and metadata
- Add versioning and related-document linking

#### Phase 3: Complaint module (Day 16–21)
- Multi-step complaint form + attachment uploads
- Tracking page + timeline
- Admin complaint queue, assignment, status transitions, SLA flags
- Notification hooks (email/SMS if available)

#### Phase 4: CMS/admin enablement (Day 22–25)
- Page/content block editor
- News/media publishing flow
- Menu management and homepage section controls

#### Phase 5: Hardening + launch (Day 26–30)
- Accessibility pass and performance optimization
- Security tests + role permission validation
- UAT with stakeholder scenarios
- Content migration + go-live checklist

### 14.9 Done criteria (must-pass)
- All public routes implemented and mobile responsive
- Complaint flow end-to-end works with unique reference IDs
- Instruments searchable/filterable with downloadable files
- Admin can edit homepage content, menus, news, and documents
- Audit log records all admin actions
- Lighthouse and accessibility targets met

### 14.10 Copy-paste master prompt for implementation agent
Use this as your one-time implementation prompt:

> Build a production-ready, premium, mobile-first official website for Niger State Electricity Regulatory Commission (NSERC) using the “Executive Civic” design direction.
> 
> Requirements:
> 1) Implement full sitemap exactly as specified:
> - Public: `/`, `/about/*`, `/regulatory-instruments*`, `/services/*`, `/resources/*`, `/news-media/*`, `/search`, `/contact`, `/privacy-policy`, `/terms-of-use`, `/accessibility`, `/404`, `/maintenance`.
> - Complaints: `/complaints/new`, `/complaints/track`, `/complaints/track/:reference`, `/complaints/checklist`, `/complaints/acknowledgement/:reference`.
> - Admin: `/admin/login`, `/admin/dashboard`, `/admin/content/pages`, `/admin/content/menus`, `/admin/media-library`, `/admin/news`, `/admin/instruments`, `/admin/documents`, `/admin/complaints`, `/admin/users-roles`, `/admin/audit-logs`, `/admin/settings`.
> 
> 2) Implement mobile-first wireframe behavior section-by-section:
> - Home: utility strip, hero with 2 CTAs, quick action cards, regulatory spotlight, consumer protection timeline, news/hearings tabs, trust block, footer.
> - Instruments list/detail: sticky search, mobile filter drawer, metadata-rich cards, version history, related instruments.
> - Complaints: 4-step form, file upload, consent, reference generation, tracking timeline, escalation guidance.
> - News/media: category tabs, featured post, list cards.
> - Contact: office cards, map, contact form.
> - Admin dashboard: KPIs, queues, audit feed, quick actions.
> 
> 3) Branding and UI:
> - Use color tokens: `#0E6B3A`, `#1C8A50`, `#C79A2B`, `#1C1C1C`, `#F7F8F6`, `#5F6B66`.
> - Typography: Manrope/Sora for headings, Inter/Source Sans for body.
> - Institutional premium style: clean spacing, restrained motion, high readability.
> 
> 4) Functional modules:
> - Complaint management: create, validate, upload evidence, issue reference, track status, admin assign/escalate/resolve.
> - Regulatory instruments engine: CRUD, publish workflow, metadata, versioning, search/filter, related links.
> - CMS/admin: manage pages, menus, hero banners, news, media/documents.
> 
> 5) Data models:
> - User, Complaint, ComplaintUpdate, Instrument, DocumentAsset, NewsPost/Event, MediaAsset, AuditLog.
> 
> 6) API contract:
> - Auth endpoints (`/api/auth/*`), complaint endpoints (`/api/complaints*`), instruments endpoints (`/api/instruments*`), CMS endpoints (`/api/pages`, `/api/menus`), upload endpoints.
> 
> 7) Non-functional constraints:
> - Lighthouse mobile performance >= 85, accessibility >= 95.
> - WCAG-compliant contrast and keyboard navigation.
> - RBAC + MFA for admins, rate limiting and captcha for complaint submission, malware scan for uploads, immutable audit logs.
> - Daily backups and uptime target 99.5%.
> 
> 8) Delivery expectations:
> - Build all features in a single implementation run.
> - Include seed data and sample content for every major page.
> - Provide migration scripts, environment setup, and README runbook.
> - Add automated tests for complaint flow, instruments filtering, and role permissions.
> - Provide final QA report showing route coverage, accessibility checks, and known limitations.

