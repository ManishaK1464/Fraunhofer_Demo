# IEM-TestGen

**Tagline:** AI-Powered Test Case Generator

https://testgen-frontend.netlify.app/

---

## Overview

IEM-TestGen is a no-login, AI-driven web application that transforms simple requirement descriptions into comprehensive, editable test cases. By leveraging Large Language Models (LLMs), it delivers an instant proof-of-concept (MVP) that saves test engineers hours of manual effort and ensures consistent, high-quality test coverage.

---

## Problem Statement

**Manual Test Creation Is Slow**  
Crafting detailed test scenarios by hand consumes significant time.

**Inconsistency and Gaps**  
Human authors often miss edge cases or apply uneven rigor.

**Maintenance Overhead**  
Keeping test documentation up to date across evolving requirements is laborious.

---

## Proposed Solution

1. **AI-Powered Generation**  
   - Parse plain-language requirements.  
   - Identify key scenarios and edge cases.  
   - Generate step-by-step test flows with expected outcomes.

2. **Inline Editing**  
   - Modify IDs, titles, descriptions, steps, priorities, and statuses directly in the table.  
   - Add or remove test cases on the fly.

3. **Instant Exports**  
   - Download CSV or copy to clipboard with one click.

4. **Zero-Friction Access**  
   - No registration or sign-up—just open the link and start generating.  
   - Responsive design for mobile and desktop.

---
## Tech Stack

- **Frontend:** React, Vite, react-i18next for localization  
- **Backend:** FastAPI, Python 3.9  
- **AI Integration:** GROQ API for AI-driven test case generation  
- **Deployment:** Netlify (frontend), Render (backend)

---