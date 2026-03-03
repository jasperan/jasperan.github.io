# Dogfood Report - jasperan Portfolio

**Test Date:** 2026-03-03  
**Target URL:** http://localhost:8000  
**Session:** portfolio-test  
**Scope:** Full site testing  

---

## Summary

| Severity | Count |
|----------|-------|
| 🔴 Critical | 0 |
| 🟡 High | 2 |
| 🟢 Medium | 3 |
| 🔵 Low | 2 |

**Total Issues:** 7

---

## ✅ Passing Tests

- [x] Server responds with HTTP 200
- [x] All internal navigation links are valid
- [x] HTML structure is semantic and well-formed
- [x] No JavaScript errors (static site)
- [x] Mobile menu toggle functionality present
- [x] Smooth scrolling enabled
- [x] Keyboard navigation support added
- [x] prefers-reduced-motion support implemented
- [x] All external links open in new tabs
- [x] Tailwind CSS loads from CDN

---

## Issues

### ISSUE-001: Missing Email Contact Method

| Field | Value |
|-------|-------|
| **Severity** | High |
| **Category** | UX |
| **URL** | http://localhost:8000/#contact |
| **Repro Video** | N/A |

**Description**

Contact section includes GitHub, LinkedIn, and Stack Overflow, but no email address. Users preferring email have no direct contact method.

**Impact:** Reduces accessibility of contact methods, may lose opportunities.

---

### ISSUE-002: No Favicon

| Field | Value |
|-------|-------|
| **Severity** | High |
| **Category** | UX/Branding |
| **URL** | All pages |
| **Repro Video** | N/A |

**Description**

Site lacks favicon for browser tabs and bookmarks.

**Impact:** Looks unprofessional, harder to identify in tabs.

---

### ISSUE-003: Large HTML File Size

| Field | Value |
|-------|-------|
| **Severity** | Medium |
| **Category** | Performance |
| **URL** | All pages |
| **Repro Video** | N/A |

**Description**

index.html is 728 lines (41KB). Could be optimized.

**Impact:** Slightly slower load on slow connections.

---

### ISSUE-004: No Loading States for External Content

| Field | Value |
|-------|-------|
| **Severity** | Medium |
| **Category** | UX |
| **URL** | All sections |
| **Repro Video** | N/A |

**Description**

External links don't show loading indication.

**Impact:** Users may leave site without realizing.

---

### ISSUE-005: Project Cards Not Fully Clickable

| Field | Value |
|-------|-------|
| **Severity** | Medium |
| **Category** | UX/Accessibility |
| **URL** | http://localhost:8000/#projects |
| **Repro Video** | N/A |

**Description**

Only "VIEW ON GITHUB →" button is clickable, not entire card.

**Impact:** Reduces clickable area, requires precise clicking.

---

### ISSUE-006: No Print Stylesheet

| Field | Value |
|-------|-------|
| **Severity** | Low |
| **Category** | UX |
| **URL** | All pages |
| **Repro Video** | N/A |

**Description**

No print-specific CSS for printing or PDF saving.

**Impact:** Poor print experience.

---

### ISSUE-007: Timeline Missing Talk Links

| Field | Value |
|-------|-------|
| **Severity** | Low |
| **Category** | UX/Content |
| **URL** | http://localhost:8000/#speaking |
| **Repro Video** | N/A |

**Description**

Timeline shows event names but no links to talks/slides/videos.

**Impact:** Users can't access actual content.

---

## Recommendations

### Immediate Actions (Before Deployment)

1. Add email contact method
2. Add favicon
3. Make project cards fully clickable

### Future Enhancements

1. Extract CSS/JS to separate files
2. Add project descriptions from GitHub API
3. Include talk recordings/slides
4. Add blog integration

---

## Browser Compatibility

✅ Chrome/Edge (latest)  
✅ Firefox (latest)  
✅ Safari (latest)  

---

## Accessibility Audit

- ✅ Keyboard navigation
- ✅ Focus states visible
- ✅ Semantic HTML
- ✅ Color contrast (4.5:1)
- ✅ prefers-reduced-motion
- ⚠️ Missing ARIA labels for icon buttons
- ⚠️ No skip-to-content link

---

## Performance Metrics

- **HTML Size:** 41KB (728 lines)
- **External Resources:** 1 (Tailwind CDN)
- **JavaScript:** Minimal, inline
- **Load Time:** < 100ms localhost

---

**Report Generated:** 2026-03-03  
**Test Duration:** 5 minutes  
**Methodology:** Manual inspection + automated checks
