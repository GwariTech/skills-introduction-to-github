# NSERC Option A (Executive Civic) — One-Time Full Implementation Prompt

Copy everything below and give it to your implementation AI agent.

---

Build a production-ready, premium, mobile-first official website for Niger State Electricity Regulatory Commission (NSERC) using the “Executive Civic” design direction.

## 1) Project objective
Create a trusted public regulatory website plus admin system where stakeholders can:
- Lodge and track complaints,
- Access regulatory instruments and public documents,
- Read news/notices/events,
- Find consumer guidance and official contact channels.

Admins must be able to:
- Update website pages, menus, hero banners, and media,
- Manage regulatory instruments lifecycle,
- Manage complaint workflow and SLA tracking,
- Publish news and notices,
- View audit logs.

## 2) Branding and design language
- Style: Premium, clean, institutional, authoritative, mobile-first.
- Color tokens:
  - Primary `#0E6B3A`
  - Secondary `#1C8A50`
  - Accent `#C79A2B`
  - Text `#1C1C1C`
  - Background `#F7F8F6`
  - Support `#5F6B66`
- Typography:
  - Headings: Manrope or Sora
  - Body: Inter or Source Sans 3
- UI behavior:
  - High readability, restrained animation, spacious layout,
  - Sticky complaint CTA,
  - High-contrast accessible controls.

## 3) Full sitemap (must implement exactly)
### Public
- `/`
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
  - `/regulatory-instruments/:slug`
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
  - `/services/license-permit-applications`
  - `/services/stakeholder-consultations`
  - `/services/clarification-requests`
- `/resources`
  - `/resources/forms-templates`
  - `/resources/download-center`
  - `/resources/faq`
  - `/resources/consumer-education`
  - `/resources/market-data-reports`
  - `/resources/procurement-tenders`
  - `/resources/careers`
- `/news-media`
  - `/news-media/press-releases`
  - `/news-media/news-updates`
  - `/news-media/events-hearings`
  - `/news-media/photo-gallery`
  - `/news-media/video-briefings`
  - `/news-media/public-notices`
  - `/news-media/:slug`
- `/search`
- `/contact`
- `/privacy-policy`
- `/terms-of-use`
- `/accessibility`
- `/404`
- `/maintenance`

### Complaints
- `/complaints/new`
- `/complaints/track`
- `/complaints/track/:reference`
- `/complaints/checklist`
- `/complaints/acknowledgement/:reference`

### Admin
- `/admin/login`
- `/admin/dashboard`
- `/admin/content/pages`
- `/admin/content/menus`
- `/admin/media-library`
- `/admin/news`
- `/admin/instruments`
- `/admin/documents`
- `/admin/complaints`
- `/admin/users-roles`
- `/admin/audit-logs`
- `/admin/settings`

## 4) Mobile wireframes (section-by-section behavior)
### Home
1. Utility strip (emergency line + office hours)
2. Header (logo, menu, complaint CTA)
3. Hero (headline, subtext, 2 CTAs)
4. Quick action cards (Lodge, Track, Forms, Latest Orders)
5. Regulatory spotlight (latest instruments)
6. Consumer protection timeline
7. News/hearings tabs
8. Trust block
9. Footer

### Instruments list
1. Heading/introduction
2. Sticky search
3. Mobile filter drawer (Type, Year, Topic, Status)
4. Sort
5. Result cards with metadata and download
6. Pagination/load more
7. Empty state

### Instrument detail
1. Breadcrumb
2. Title + type/status badges
3. Metadata table
4. Summary
5. Download/view actions
6. Version history
7. Related instruments
8. Share/print

### Complaint submit
1. Intro + timelines
2. 4-step form (identity, details, upload, review)
3. Validation and guided fields
4. Consent + privacy
5. Generate reference on successful submission

### Complaint track
1. Reference + verification input
2. Status timeline
3. Updates/messages
4. Download acknowledgement/resolution
5. Escalation guidance

### News/media
1. Category tabs
2. Featured story
3. List cards
4. Date/keyword filter

### Contact
1. Office cards
2. Map
3. Contact form
4. Complaint redirect note

### Admin dashboard
1. KPI cards
2. Work queues
3. Audit feed
4. Quick actions

## 5) Functional modules
### Complaint management
- Public submit + track + evidence upload.
- Auto unique complaint ID.
- Admin assignment, status changes, escalations, SLA monitoring, outcome letter.

### Regulatory instruments engine
- CRUD with draft/review/publish/archive.
- Metadata-driven search/filter.
- Versioning and related-document links.
- File downloads.

### CMS/admin
- Edit pages, menus, banners, writeups, images.
- Publish news/notices/events.
- Role-based controls + audit log.

## 6) Data model
- User
- Complaint
- ComplaintUpdate
- Instrument
- DocumentAsset
- NewsPost/Event
- MediaAsset
- AuditLog

## 7) API contract (minimum)
- Auth: `/api/auth/login`, `/api/auth/logout`, `/api/auth/me`
- Complaints: create, track, add messages, admin status update
- Instruments: list, detail, admin create/update/publish
- CMS: page read/update, menu read/update
- Uploads/documents endpoints

## 8) Non-functional requirements
- Lighthouse mobile performance >= 85
- Lighthouse accessibility >= 95
- WCAG-compliant contrast and keyboard navigation
- RBAC + MFA for admin users
- Rate limiting + captcha for complaint endpoint
- Anti-malware file scanning
- Immutable audit logs
- Daily backups and 99.5% uptime target

## 9) One-time implementation plan (single run)
- Day 1–3: foundation (architecture, tokens, base layout, auth)
- Day 4–10: public pages and navigation
- Day 11–15: instruments engine
- Day 16–21: complaints module
- Day 22–25: CMS/admin completion
- Day 26–30: QA hardening, accessibility/performance/security, go-live

## 10) Done criteria
- Every route implemented and responsive.
- Complaint flow works end-to-end with reference generation and tracking.
- Instruments searchable/filterable with downloads and versioning.
- Admin can manage content, menus, media, instruments, complaints.
- Audit logs capture admin actions.
- Meets performance and accessibility targets.

## 11) Delivery format expected from implementation agent
- Full source code
- Database migrations + seed data
- Environment setup + README runbook
- Automated tests (complaints flow, instrument filtering, role permissions)
- Final QA report with known limitations

---

If anything is unclear, the implementation agent must proceed with best-practice assumptions and explicitly document those assumptions in the README.
