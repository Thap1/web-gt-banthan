---
stepsCompleted: [1, 2, 3, 4, 7, 8, 9, 10, 11]
inputDocuments: []
workflowType: 'prd'
lastStep: 11
project_name: 'web-gt-banthan'
user_name: 'Thap'
date: '2025-12-07'
portfolio_owner: 'Lê Huyền'
status: 'complete'
completedAt: '2025-12-07'
---

# Product Requirements Document - web-gt-banthan

**Author:** Thap
**Date:** 2025-12-07
**Portfolio Owner:** Lê Huyền

## Executive Summary

Portfolio CV online dành cho **Lê Huyền** (Tester) - một web application được Thap xây dựng để giúp Lê Huyền showcase bản thân một cách chuyên nghiệp khi đi phỏng vấn. Thay vì CV tĩnh truyền thống, web này cung cấp trải nghiệm tương tác, luôn cập nhật, và thể hiện sự chuyên nghiệp của một QA/Tester.

### What Makes This Special

- **Professional presentation**: Portfolio web chuyên nghiệp tạo ấn tượng tốt với nhà tuyển dụng
- **Dynamic content management**: CRUD cho tất cả sections, Lê Huyền dễ dàng cập nhật mà không cần redeploy
- **Professional depth**: Blog chia sẻ kiến thức + Testimonials từ đồng nghiệp tạo social proof
- **Convenience**: Download CV PDF giúp HR lưu trữ theo quy trình truyền thống

## Project Classification

**Technical Type:** Web Application (SPA)
**Domain:** General/Portfolio
**Complexity:** Low

Project thuộc dạng web app cá nhân với yêu cầu kỹ thuật chuẩn. Không có quy định đặc thù về compliance hay domain-specific requirements. Focus chính vào UX, performance và khả năng quản lý nội dung linh hoạt.

## Success Criteria

### User Success (Nhà tuyển dụng / HR)

- **First Impression**: Trong 5 giây đầu, HR hiểu ngay Lê Huyền là Tester với bao nhiêu năm kinh nghiệm
- **Information Discovery**: Tìm được thông tin cần thiết (skills, experience, projects) trong vòng 30 giây
- **Credibility Signal**: Ấn tượng với portfolio web chuyên nghiệp
- **Convenience**: Download được CV PDF chỉ với 1 click

### User Success (Admin - Lê Huyền)

- **Easy Updates**: Cập nhật bất kỳ nội dung nào trong vòng 2 phút, không cần code
- **Full Control**: CRUD tất cả sections mà không cần hỗ trợ kỹ thuật
- **Always Current**: Portfolio luôn reflect thông tin mới nhất

### Business Success

- **Interview Ready**: Portfolio sẵn sàng gửi cho nhà tuyển dụng trong hôm nay
- **Conversation Starter**: Nhà tuyển dụng đề cập đến portfolio trong buổi phỏng vấn
- **Professional Image**: Lê Huyền có công cụ showcase chuyên nghiệp

### Technical Success

- **Performance**: Trang load dưới 3 giây trên 3G connection
- **Responsive**: Hiển thị tốt trên mobile, tablet, desktop
- **SEO Friendly**: Có thể tìm thấy qua Google search tên Lê Huyền
- **Uptime**: Deploy trên Vercel với 99.9% uptime (free tier)

### Measurable Outcomes

| Metric | Target |
|--------|--------|
| Page Load Time | < 3s |
| Time to First Content | < 1s |
| Mobile Lighthouse Score | > 80 |
| Admin CRUD Operation | < 30s mỗi action |
| CV PDF Generation | < 5s |

## Product Scope

### MVP - Minimum Viable Product (Hôm nay - 8 tiếng)

**Public Portfolio:**
- Hero section (ảnh, tên, title, intro)
- About section
- Skills (testing tools, languages, methodologies)
- Experience (timeline công việc)
- Projects (dự án đã tham gia)
- Certifications
- Education
- Contact + Download CV PDF

**Admin Panel:**
- Authentication (login bảo vệ admin)
- CRUD cho tất cả sections trên

### Growth Features (Post-MVP)

- Blog section với CRUD
- Testimonials từ đồng nghiệp
- Analytics dashboard (views, downloads)
- Dark mode toggle
- Multi-language support

### Vision (Future)

- AI-powered CV customization theo job description
- Integration với LinkedIn import
- Multiple CV templates
- Scheduling cho content publishing

## User Journeys

### Journey 1: Minh Anh - HR Manager Tìm Kiếm Tester

Minh Anh là HR Manager tại một công ty fintech đang scale nhanh. Team QA cần thêm 2 Senior Tester gấp nhưng đã 3 tuần mà chưa tìm được ứng viên phù hợp. Các CV nhận được đều giống nhau - liệt kê skills và công ty cũ, không có gì nổi bật.

Một buổi chiều, Minh Anh nhận được email ứng tuyển từ Lê Huyền với link portfolio thay vì file PDF đính kèm. Tò mò, cô click vào. Ngay lập tức, cô thấy một trang web chuyên nghiệp với ảnh, title "QA Engineer | 5 Years Experience", và một intro ngắn gọn súc tích.

Scroll xuống, Minh Anh thấy timeline kinh nghiệm được trình bày rõ ràng - không chỉ tên công ty mà còn có mô tả cụ thể về testing methodologies đã áp dụng. Phần Projects liệt kê các dự án thực tế với tech stack và vai trò. Điều khiến cô ấn tượng nhất: ứng viên này có một portfolio web chuyên nghiệp - chứng minh sự nghiêm túc trong công việc.

Cô click "Download CV" để lưu vào hồ sơ, rồi schedule phỏng vấn ngay trong ngày.

**Journey Requirements:**
- Hero section hiển thị ngay thông tin quan trọng nhất
- Timeline experience dễ scan
- Projects với context rõ ràng
- One-click CV download
- Mobile responsive (HR có thể xem trên điện thoại)

---

### Journey 2: Lê Huyền - Cập Nhật Portfolio Trước Phỏng Vấn

Lê Huyền vừa nhận được lịch phỏng vấn cho vị trí Senior QA tại một công ty healthcare. Cô nhận ra portfolio hiện tại chưa highlight kinh nghiệm với testing trong lĩnh vực regulated industries.

Lê Huyền mở laptop, truy cập admin panel và login. Dashboard hiện ra với danh sách tất cả sections. Cô click vào "Experience" và thêm một bullet point về compliance testing đã làm ở công ty cũ. Tiếp theo, cô vào "Skills" và thêm "HIPAA Compliance Testing" vào danh sách.

Cuối cùng, cô vào "Projects" và edit một project cũ để highlight phần security testing. Tất cả chỉ mất 10 phút. Cô refresh trang public và thấy thay đổi đã live ngay lập tức.

Tự tin với portfolio đã cập nhật, Lê Huyền gửi link cho HR và chuẩn bị cho buổi phỏng vấn.

**Journey Requirements:**
- Secure login cho admin
- Dashboard với list tất cả sections
- Edit inline nhanh chóng
- Changes reflect ngay lập tức
- No redeploy needed

---

### Journey 3: Lê Huyền - Thêm Project Mới

Lê Huyền vừa hoàn thành một dự án lớn và muốn thêm vào portfolio. Cô login vào admin, navigate đến "Projects", và click "Add New".

Form hiện ra với các fields: Project Name, Description, Technologies, Role, Duration, và Achievements. Cô điền từng field, upload một screenshot (optional), và click Save.

Project mới xuất hiện ngay trên trang public, được sắp xếp theo thời gian mới nhất trước.

**Journey Requirements:**
- CRUD đầy đủ cho Projects
- Form với validation
- Image upload support
- Auto-sort by date

---

### Journey 4: Visitor - Xem Portfolio Trên Mobile

Một Tech Lead đang ngồi cafe và nhận được link portfolio của Lê Huyền qua LinkedIn message. Anh mở trên điện thoại.

Trang load nhanh, hiển thị tốt trên màn hình nhỏ. Navigation collapse thành hamburger menu. Anh scroll qua từng section, tap vào một project để xem chi tiết, rồi tap "Download CV" để lưu về máy.

Ấn tượng với portfolio, anh forward link cho HR team với note "Check this candidate".

**Journey Requirements:**
- Mobile-first responsive design
- Fast loading (< 3s on 3G)
- Touch-friendly navigation
- PDF download works on mobile

---

### Journey Requirements Summary

| Capability | Related Journeys |
|------------|-----------------|
| Hero Section Display | Journey 1, 4 |
| Experience Timeline | Journey 1 |
| Projects Showcase | Journey 1, 3, 4 |
| Skills Display | Journey 2 |
| CV PDF Download | Journey 1, 4 |
| Admin Authentication | Journey 2, 3 |
| CRUD All Sections | Journey 2, 3 |
| Real-time Updates | Journey 2 |
| Mobile Responsive | Journey 4 |
| Fast Performance | Journey 4 |

## Web Application Specific Requirements

### Project-Type Overview

Portfolio web application sử dụng kiến trúc SPA với Next.js 14 App Router. Hybrid rendering (SSR cho SEO, CSR cho admin interactions). Single-user system với một admin account.

### Browser Support Matrix

| Browser | Minimum Version | Notes |
|---------|-----------------|-------|
| Chrome | Latest 2 versions | Primary target |
| Firefox | Latest 2 versions | Full support |
| Safari | Latest 2 versions | iOS/macOS users |
| Edge | Latest 2 versions | Windows users |
| Mobile Chrome | Latest | Android users |
| Mobile Safari | Latest | iOS users |

**Not Supported:** Internet Explorer, Opera Mini

### Responsive Design Requirements

| Breakpoint | Width | Target Devices |
|------------|-------|----------------|
| Mobile | < 640px | Phones |
| Tablet | 640px - 1024px | Tablets, small laptops |
| Desktop | > 1024px | Laptops, monitors |

**Design Approach:** Mobile-first responsive design với Tailwind CSS

### Performance Targets

| Metric | Target | Measurement Tool |
|--------|--------|------------------|
| First Contentful Paint | < 1.5s | Lighthouse |
| Largest Contentful Paint | < 2.5s | Lighthouse |
| Time to Interactive | < 3.0s | Lighthouse |
| Cumulative Layout Shift | < 0.1 | Lighthouse |
| Lighthouse Performance Score | > 80 | Lighthouse |

**Optimization Strategies:**
- Image optimization với Next.js Image component
- Code splitting per route
- Static generation cho public pages
- Lazy loading cho below-the-fold content

### SEO Strategy

| Requirement | Implementation |
|-------------|----------------|
| Meta tags | Dynamic per page với Next.js Metadata API |
| Open Graph | Full OG tags cho social sharing |
| Sitemap | Auto-generated sitemap.xml |
| Robots.txt | Allow all crawlers |
| Structured Data | JSON-LD cho Person schema |
| Canonical URLs | Self-referencing canonicals |

### Accessibility Level

**Target:** WCAG 2.1 Level AA (Basic Compliance)

| Requirement | Implementation |
|-------------|----------------|
| Keyboard Navigation | All interactive elements focusable |
| Screen Reader | Semantic HTML, ARIA labels where needed |
| Color Contrast | Minimum 4.5:1 for text |
| Focus Indicators | Visible focus rings |
| Alt Text | All images have descriptive alt text |

### Testing Requirements

**Testing Strategy:** Comprehensive testing với automated scripts - showcase QA expertise

#### Unit Tests

| Area | Tool | Coverage Target |
|------|------|-----------------|
| Components | Jest + React Testing Library | > 80% |
| API Routes | Jest | 100% |
| Utilities | Jest | 100% |

**Test Cases Examples:**
- Hero component renders correct data
- Skills list displays all items
- Experience timeline sorts correctly
- Form validation works as expected

#### Integration Tests

| Area | Tool | Scope |
|------|------|-------|
| API CRUD | Jest + Supertest | All endpoints |
| Auth Flow | Jest | Login/Logout |
| Data Flow | Jest | DB to UI |

**Test Cases Examples:**
- Create new project → appears in list
- Update experience → changes reflect on public page
- Delete skill → removed from display

#### E2E Tests (Automation Scripts)

| Tool | Scope | Priority |
|------|-------|----------|
| Playwright | Critical user journeys | P0 |

**Automation Test Scenarios:**

| Test ID | Scenario | Steps |
|---------|----------|-------|
| E2E-001 | Visitor views portfolio | Navigate → Scroll sections → Verify content |
| E2E-002 | Download CV PDF | Click download → Verify file downloaded |
| E2E-003 | Admin login | Enter credentials → Verify dashboard access |
| E2E-004 | CRUD Experience | Login → Add/Edit/Delete experience → Verify changes |
| E2E-005 | CRUD Projects | Login → Add project with image → Verify on public |
| E2E-006 | CRUD Skills | Login → Add/Edit/Delete skill → Verify display |
| E2E-007 | Mobile responsive | Resize viewport → Verify layout adapts |
| E2E-008 | Performance check | Run Lighthouse → Verify score > 80 |

#### Test Documentation

Mỗi feature cần đi kèm:
- Test case document (Given/When/Then format)
- Automation script (Playwright)
- Test data setup/teardown

**Thư mục cấu trúc:**
```
/tests
  /unit           → Jest unit tests
  /integration    → API integration tests
  /e2e            → Playwright E2E tests
  /fixtures       → Test data
  /reports        → Test reports output
```

### Implementation Considerations

**Tech Stack Decisions:**
- **Framework:** Next.js 14 với App Router
- **Styling:** Tailwind CSS + shadcn/ui components
- **Database:** SQLite với Prisma ORM
- **Auth:** NextAuth.js với credentials provider
- **Hosting:** Vercel (free tier)
- **PDF Generation:** react-pdf hoặc html2pdf.js
- **Testing:** Jest + React Testing Library + Playwright

**Architecture:**
```
/app
  /(public)        → Public portfolio pages (SSG)
  /admin           → Protected admin pages (CSR)
  /api             → API routes cho CRUD operations
/prisma
  schema.prisma    → Database schema
/components
  /ui              → shadcn/ui components
  /sections        → Portfolio section components
/tests
  /unit            → Unit tests
  /e2e             → Playwright tests
```

## Project Scoping & Phased Development

### MVP Strategy & Philosophy

**MVP Approach:** Problem-Solving MVP
- Giải quyết core problem: Lê Huyền cần portfolio chuyên nghiệp để đi phỏng vấn
- Minimal features, maximum impact
- Focus: Hoàn thành trong 8 tiếng

**Resource Requirements:**
- 1 Developer (Thap)
- Timeline: 8 giờ
- Tech: Next.js + SQLite + Tailwind

### MVP Feature Set (Phase 1 - Hôm nay)

**Core User Journeys Supported:**
- Journey 1: HR views portfolio (public view)
- Journey 2: Lê Huyền updates content (admin CRUD)
- Journey 3: Add new project (admin CRUD)
- Journey 4: Mobile viewing (responsive)

**Must-Have Capabilities:**

| Feature | Priority | Time Est. |
|---------|----------|-----------|
| Project Setup (Next.js + Prisma + Auth) | P0 | 1h |
| Public Portfolio - All Sections | P0 | 2h |
| Admin Authentication | P0 | 30min |
| Admin CRUD Dashboard | P0 | 3h |
| CV PDF Download | P0 | 1h |
| Basic Unit Tests | P1 | 30min |

**MVP Testing Scope:**
- Smoke tests cho critical paths
- Basic unit tests cho CRUD operations
- Manual testing cho UI/UX

### Post-MVP Features

**Phase 2 (Post-MVP - Tuần sau):**
- Blog section với CRUD
- Testimonials section
- Comprehensive E2E tests (Playwright)
- Full unit test coverage (>80%)

**Phase 3 (Expansion - Tháng sau):**
- Analytics dashboard
- Dark mode toggle
- Multi-language support
- CI/CD với automated testing

**Phase 4 (Vision - Tương lai):**
- AI-powered CV customization
- LinkedIn import
- Multiple CV templates

### Risk Mitigation Strategy

**Technical Risks:**

| Risk | Mitigation |
|------|------------|
| PDF generation complexity | Use html2pdf.js (simple, client-side) |
| SQLite limitations | Sufficient for single-user, migrate later if needed |
| Time overrun | Strict MVP scope, defer testing to Phase 2 |

**Market Risks:**
- Low risk - personal portfolio, không có external dependencies

**Resource Risks:**

| Risk | Contingency |
|------|-------------|
| < 8 giờ available | Defer Blog/Testimonials to Phase 2 |
| Technical blockers | Use simpler alternatives (JSON files instead of DB) |

### MVP Acceptance Criteria

Portfolio MVP được coi là DONE khi:
1. Public portfolio hiển thị tất cả sections
2. Admin có thể CRUD tất cả content
3. CV PDF download hoạt động
4. Responsive trên mobile
5. Deploy thành công trên Vercel
6. Smoke tests pass

## Functional Requirements

### Public Portfolio Display

- FR1: Visitor can view hero section with profile photo, name, title, and intro
- FR2: Visitor can view about section with detailed personal introduction
- FR3: Visitor can view skills organized by categories (testing tools, languages, methodologies)
- FR4: Visitor can view experience timeline sorted by date (newest first)
- FR5: Visitor can view project cards with name, description, technologies, role, and achievements
- FR6: Visitor can view certifications list with name, issuer, and date
- FR7: Visitor can view education history with institution, degree, and graduation year
- FR8: Visitor can view contact information section
- FR9: Visitor can navigate between sections using menu/navigation
- FR10: Visitor can view portfolio on mobile devices with responsive layout

### CV Download

- FR11: Visitor can download CV as PDF with one click
- FR12: System generates PDF containing all portfolio content in printable format

### Admin Authentication

- FR13: Admin can login with username and password
- FR14: Admin can logout from admin panel
- FR15: System protects admin routes from unauthorized access
- FR16: System maintains admin session across page refreshes

### Content Management - Profile

- FR17: Admin can update hero section content (photo, name, title, intro)
- FR18: Admin can update about section content

### Content Management - Skills

- FR19: Admin can view list of all skills
- FR20: Admin can add new skill with name and category
- FR21: Admin can edit existing skill
- FR22: Admin can delete skill
- FR23: Admin can organize skills by category

### Content Management - Experience

- FR24: Admin can view list of all experiences
- FR25: Admin can add new experience with company, role, duration, and description
- FR26: Admin can edit existing experience
- FR27: Admin can delete experience
- FR28: System auto-sorts experiences by date

### Content Management - Projects

- FR29: Admin can view list of all projects
- FR30: Admin can add new project with name, description, technologies, role, duration, and achievements
- FR31: Admin can upload project screenshot/image
- FR32: Admin can edit existing project
- FR33: Admin can delete project
- FR34: System auto-sorts projects by date

### Content Management - Certifications

- FR35: Admin can view list of all certifications
- FR36: Admin can add new certification with name, issuer, and date
- FR37: Admin can edit existing certification
- FR38: Admin can delete certification

### Content Management - Education

- FR39: Admin can view list of all education entries
- FR40: Admin can add new education with institution, degree, field, and graduation year
- FR41: Admin can edit existing education entry
- FR42: Admin can delete education entry

### Content Management - Contact

- FR43: Admin can update contact information (email, phone, LinkedIn, etc.)

### Data Persistence

- FR44: System persists all content changes to database
- FR45: System reflects content changes on public portfolio immediately after save
- FR46: System maintains data integrity across all CRUD operations

### Testing Capabilities

- FR47: System provides testable API endpoints for all CRUD operations
- FR48: System supports automated testing via Playwright
- FR49: System provides test data seeding capability

## Non-Functional Requirements

### Performance

- NFR1: Public pages load within 3 seconds on 3G connection
- NFR2: First Contentful Paint (FCP) occurs within 1.5 seconds
- NFR3: Largest Contentful Paint (LCP) occurs within 2.5 seconds
- NFR4: Time to Interactive (TTI) is under 3 seconds
- NFR5: Cumulative Layout Shift (CLS) is below 0.1
- NFR6: Lighthouse Performance score is above 80
- NFR7: Admin CRUD operations complete within 2 seconds
- NFR8: CV PDF generation completes within 5 seconds
- NFR9: Image uploads complete within 10 seconds for files up to 5MB

### Security

- NFR10: Admin credentials are hashed using bcrypt or similar secure algorithm
- NFR11: Admin sessions expire after 24 hours of inactivity
- NFR12: Admin routes are protected and redirect unauthorized access to login
- NFR13: API endpoints validate input and sanitize against XSS attacks
- NFR14: Database connections use parameterized queries to prevent SQL injection
- NFR15: HTTPS is enforced for all traffic
- NFR16: Environment variables store sensitive configuration (not hardcoded)

### Accessibility

- NFR17: All interactive elements are keyboard accessible
- NFR18: Color contrast ratio meets WCAG 2.1 AA standard (4.5:1 for text)
- NFR19: All images have descriptive alt text
- NFR20: Form inputs have associated labels
- NFR21: Focus indicators are visible on all interactive elements
- NFR22: Page structure uses semantic HTML elements
- NFR23: Site is navigable by screen readers

### Reliability

- NFR24: System maintains 99.9% uptime (Vercel SLA)
- NFR25: Database operations are atomic (no partial writes)
- NFR26: System gracefully handles errors with user-friendly messages
- NFR27: Data is preserved if browser closes during admin edit
- NFR28: System recovers automatically from temporary network failures

### Maintainability

- NFR29: Codebase follows consistent coding standards (ESLint + Prettier)
- NFR30: Components are modular and reusable
- NFR31: API endpoints follow RESTful conventions
- NFR32: Database schema supports future extensions without breaking changes
- NFR33: Test coverage enables confident refactoring

