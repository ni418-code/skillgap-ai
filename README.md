# SkillGap AI

> **Know. Learn. Build. Prove. Get Ready.**

SkillGap AI is an AI-powered opportunity readiness platform designed to help students and early-career candidates understand what a target internship or job requires, identify their skill and evidence gaps, create a focused learning plan, practice the missing skills, and prove their readiness.

## Core Product Flow

```text
Profile
   ↓
Resume Analysis
   ↓
GitHub Repository Analysis
   ↓
Opportunity / Job Description Analysis
   ↓
Requirement Mapping
   ↓
Skill + Evidence + Readiness Gaps
   ↓
Prioritize
   ↓
Personalized Learning Plan
   ↓
Resources
   ↓
Practice
   ↓
Assessment
   ↓
Evidence
   ↓
Reassess
```

The product is designed around one principle:

> **Do not just tell a user what skills they need. Show what they already have, what evidence supports it, what is missing, what to learn next, and how to prove it.**

---

## 🚀 Key Features

### 1. Profile & Onboarding
Users can create a career-readiness profile containing:

- Name and contact information
- College / university
- Degree and specialization
- Current year and graduation year
- CGPA, when provided
- Target roles and domains
- Preferred industries
- Internship / job / placement goals
- Learning availability
- Preferred learning format

### 2. Resume Analysis

Users can upload a resume and extract information from the actual document.

The system is designed to identify:

- Skills
- Education
- Projects
- Experience
- Certifications
- Achievements
- Relevant resume sections

Supported document types in the prototype include:

- PDF
- DOC
- DOCX

The extracted information is mapped into the user's profile instead of replacing it with sample data.

The system should never invent resume information.

### 3. GitHub Repository Analysis

Users can enter their GitHub username and import their public repositories.

The GitHub analysis is designed to inspect:

- Repository names
- Repository descriptions
- Programming languages
- Topics / metadata
- README documentation
- Project activity
- Repository-level technology signals
- Project-to-skill relationships

Repositories are treated as **evidence signals**, not automatic proof of expertise.

For example:

```text
Repository
   ↓
Technologies / Languages
   ↓
Project Context
   ↓
Skill Signals
   ↓
Evidence
```

This avoids the simplistic assumption that:

> "Python appears in a repository → user is an expert in Python."

### 4. Opportunity Analysis

Users can add a target opportunity by providing:

- Company
- Role
- Job description
- Official opportunity URL
- Opportunity type

The analyzer separates:

- Required skills
- Preferred skills
- Responsibilities
- Technologies
- Knowledge areas
- Role-specific requirements

The requirements are then compared against the user's profile and evidence.

### 5. Skill Gap Analysis

Skill gaps are evaluated at the opportunity level.

The system distinguishes between:

#### Skill Gap
The user does not currently demonstrate the required knowledge.

#### Evidence Gap
The user may know the skill but does not have enough supporting evidence.

#### Readiness Gap
The user understands the concept but has not demonstrated practical ability.

---

## 🧠 Evidence Model

SkillGap AI uses four evidence states:

| State | Meaning |
|---|---|
| **CLAIMED** | User says they know the skill |
| **DETECTED** | Skill appears in resume, project or profile data |
| **TESTED** | Assessment supports the user's knowledge |
| **DEMONSTRATED** | Practical evidence supports the skill |

The objective is to move important skills toward:

```text
CLAIMED
   ↓
DETECTED
   ↓
TESTED
   ↓
DEMONSTRATED
```

---

## 📊 Overview Dashboard

The Overview page acts as the user's command center.

It should provide a clear picture of:

- Target opportunity
- Requirement coverage
- Evidence coverage
- Assessment coverage
- Practical demonstration
- Strong skills
- Partial skills
- Missing skills
- Top priorities
- Current learning progress
- Current readiness stage
- Recommended next action

The dashboard follows the journey:

```text
Profile
  → Analyzed
  → Gaps Found
  → Learning
  → Practicing
  → Proving
  → Reassessed
```

---

## 🎯 Role-Specific Skills

Skills are not shown as a generic global list.

The platform connects skills to the user's selected:

- Role
- Domain
- Opportunity
- Required level

For example:

```text
AI / ML Engineer
├── Python
├── Machine Learning
├── Statistics
├── Model Evaluation
├── Data Processing
├── Deep Learning
├── APIs
└── Deployment
```

A different opportunity can produce a different skill map.

---

## 📚 Personalized Learning

Learning is connected directly to the identified skill gaps.

The platform supports different learning horizons:

- 3 days
- 1 week
- 2 weeks
- 1 month
- 3 months
- 6 months

Possible learning modes include:

- Fast Track
- Practical Learning
- Deep Learning
- Interview Preparation

The learning plan should answer:

1. What should I learn?
2. Why is it required for this role?
3. What level do I need?
4. What do I already know?
5. What am I missing?
6. What should I learn first?
7. How long should it take?
8. What should I build?
9. How can I prove the skill?

---

## 🌐 Resources

Resources are selected according to:

- Target role
- Missing skill
- Required level
- Current level
- Available learning time
- Learning mode
- Preferred format
- Practical relevance

Example trusted sources:

- Microsoft Learn
- Google ML Crash Course
- Kaggle Learn
- Hugging Face
- MDN
- freeCodeCamp
- GitHub Skills
- AWS Skill Builder
- Official documentation

The product should distinguish between:

- FREE
- FREEMIUM
- PAID

It should not falsely label paid resources as free.

---

## 🛠️ Practice

High-priority gaps can lead to practical assignments.

Example:

```text
Skill Gap:
Machine Learning Model Evaluation

Practice:
Build a binary classification model.

Requirements:
✓ Load a real dataset
✓ Clean the data
✓ Split train/test data
✓ Train a model
✓ Evaluate the model
✓ Generate a confusion matrix
✓ Document the results
✓ Create a README
✓ Push the project to GitHub
```

The objective is to turn learning into evidence.

---

## 📝 Assessments

Assessments can include:

- Multiple-choice questions
- Concept questions
- Scenario questions
- Coding questions
- Practical tasks

Assessment results identify:

- Strengths
- Weak areas
- Recommended next action

A test score alone is **not treated as practical proof**.

---

## 🔎 Evidence

Evidence can come from:

- Resume
- GitHub repositories
- Projects
- Certifications
- Assessments
- Practical assignments

The evidence system connects:

```text
Opportunity Requirement
        ↓
Required Skill
        ↓
User Evidence
        ↓
Evidence Strength
        ↓
Readiness
```

---

## 🎨 UI / UX Direction

SkillGap AI is designed as a visual career-readiness experience rather than a plain dashboard.

### Landing experience

The central visual metaphor is:

```text
CONFUSED
   ↓
ANALYZED
   ↓
AWARE
   ↓
LEARNING
   ↓
PRACTICING
   ↓
PROVING
   ↓
READY
```

The landing page uses a futuristic portal/transformation concept:

- Confused student
- Skill uncertainty
- Opportunity requirements
- Analysis portal
- Learning transformation
- Project evidence
- Confident / opportunity-ready student

### Application interface

The internal application combines:

- Glass cards
- Visual progress paths
- Repository cards
- Skill maps
- Learning timelines
- Evidence indicators
- Data visualizations
- Progress animations
- Responsive layouts
- Motion transitions
- Mobile-friendly layouts

The UI should avoid becoming a collection of flat dark boxes.

---

## 🏗️ Suggested Production Architecture

### Frontend

- React
- Vite
- Tailwind CSS
- Framer Motion
- Lucide Icons
- Recharts

### Backend

- Python
- FastAPI

### AI / NLP

- LLM API
- spaCy
- Sentence Transformers
- scikit-learn

### Resume Processing

- PyMuPDF
- python-docx
- OCR fallback for scanned documents

### Database

- Supabase
- PostgreSQL

### Deployment

- Vercel — frontend
- Render — backend
- Supabase — database

### Security

API keys must remain server-side.

Production implementation should include:

- Authentication
- Authorization
- Input validation
- File validation
- Sanitized uploads
- Secure GitHub authentication
- Rate limiting
- Protected user data
- Server-side API calls

---

## 🧪 Prototype vs Production

The current HTML prototype demonstrates the product experience and interaction flow.

For production, the following should be moved to the backend:

- Resume parsing
- OCR
- LLM analysis
- GitHub repository analysis
- Opportunity extraction
- Resource retrieval
- Personalized plan generation
- Assessment generation
- Evidence scoring
- Persistent user data
- Authentication
- Opportunity monitoring

The frontend should consume secure backend APIs instead of exposing credentials.

---

## 📁 Project Structure

A production version can use:

```text
skillgap-ai/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── hooks/
│   │   └── data/
│   └── package.json
│
├── backend/
│   ├── app/
│   │   ├── api/
│   │   ├── models/
│   │   ├── services/
│   │   ├── analyzers/
│   │   └── main.py
│   └── requirements.txt
│
├── README.md
└── .gitignore
```

---

## ▶️ Running the Current Prototype

The current prototype is a standalone HTML application.

Open:

```text
skillgap-ai-portal-no-quick-reference.html
```

in a modern browser.

No frontend build step is required for the standalone prototype.

For the production architecture, use the React + FastAPI structure described above.

---

## 🔐 Environment Variables

Never commit API keys or service credentials.

Example:

```env
OPENAI_API_KEY=
GITHUB_TOKEN=
SUPABASE_URL=
SUPABASE_ANON_KEY=
SUPABASE_SERVICE_ROLE_KEY=
```

Add environment files to `.gitignore`:

```gitignore
.env
.env.*
!.env.example
```

---

## 🏆 Hackathon Value Proposition

SkillGap AI addresses a common career-readiness problem:

> Students have information, but they often lack a clear, opportunity-specific path from their current profile to demonstrable readiness.

Instead of functioning only as a resume checker, SkillGap AI connects:

**Opportunity → Requirements → Profile → Evidence → Gaps → Learning → Practice → Proof → Reassessment**

This makes the product useful beyond resume optimization.

---

## 🔮 Future Extensions

Potential future capabilities include:

- GitHub OAuth
- Private repository analysis with authorization
- Continuous opportunity monitoring
- Requirement-change detection
- Multiple opportunity comparison
- AI-generated practical projects
- Skill dependency graphs
- Portfolio recommendations
- Interview preparation
- Recruiter-facing evidence reports
- Skill progression history
- Learning streaks
- Team / mentor dashboards
- Browser extension for opportunity analysis

---

## 📌 Product Principle

SkillGap AI should never simply say:

> "You are missing Python."

It should answer:

> **What does the role require?  
> What do you already have?  
> What evidence supports it?  
> What is missing?  
> How important is the gap?  
> What should you learn?  
> How long will it take?  
> What should you build?  
> How can you prove it?**

That is the core product experience.
