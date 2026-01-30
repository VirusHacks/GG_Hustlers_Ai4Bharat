# 📋 Requirements Specification — Edify-AI

> **Version:** 1.0  
> **Last Updated:** January 25, 2026  
> **Status:** Active Development

---

## 🎯 Product Overview

### Vision Statement
**Edify-AI is "Google Maps for a Student's Career"** — an AI-powered career advisor that transforms confused, overwhelmed students into confident, job-ready professionals by providing personalized direction, guidance, and continuous correction throughout their career journey.

### Problem Statement
Today's students face critical challenges:
- **Lack of direction**: Don't know what to learn next
- **Information overload**: Open 50 tabs, watch random tutorials
- **Mismatched learning**: Buy courses that don't match their level
- **Poor job preparation**: Apply to jobs without understanding the role
- **Interview failures**: Fail interviews despite knowing the basics

> The issue is **not effort** — it's **lack of direction**.

### Target Users
| User Segment | Description | Primary Needs |
|--------------|-------------|---------------|
| **Students** | College students & recent graduates | Career clarity, skill development, job readiness |
| **Career Changers** | Professionals transitioning roles | Skill gap identification, reskilling paths |
| **Colleges/Institutions** | Placement cells & career services | Scalable career guidance, placement analytics |

---

## 📦 Functional Requirements

### FR-1: User Authentication & Profile Management
| ID | Requirement | Priority | Status |
|----|-------------|----------|--------|
| FR-1.1 | Users shall authenticate via Kinde Auth (OAuth providers) | P0 | ✅ Done |
| FR-1.2 | System shall create and maintain user profiles with skills, interests, occupation, and goals | P0 | ✅ Done |
| FR-1.3 | Users shall be able to upload and manage multiple resumes | P0 | ✅ Done |
| FR-1.4 | System shall support browser extension authentication | P1 | ✅ Done |

### FR-2: ATS Resume Analysis (Multi-Agent System)
| ID | Requirement | Priority | Status |
|----|-------------|----------|--------|
| FR-2.1 | System shall analyze resumes against job descriptions using 5 specialized AI agents | P0 | ✅ Done |
| FR-2.2 | Skills Agent shall identify matching/missing technical and soft skills | P0 | ✅ Done |
| FR-2.3 | Experience Agent shall evaluate work experience relevance | P0 | ✅ Done |
| FR-2.4 | Education Agent shall assess educational qualifications alignment | P0 | ✅ Done |
| FR-2.5 | Projects Agent shall analyze project relevance to job requirements | P0 | ✅ Done |
| FR-2.6 | Meta Agent shall evaluate seniority, domains, and language fit | P0 | ✅ Done |
| FR-2.7 | System shall provide weighted aggregate matching scores | P0 | ✅ Done |
| FR-2.8 | System shall generate actionable improvement suggestions | P0 | ✅ Done |

### FR-3: Personalized Career Roadmap
| ID | Requirement | Priority | Status |
|----|-------------|----------|--------|
| FR-3.1 | System shall generate personalized career roadmaps based on user profile | P0 | ✅ Done |
| FR-3.2 | Roadmaps shall incorporate ATS skill gaps when available | P0 | ✅ Done |
| FR-3.3 | System shall allow customization of timeframes (3mo, 6mo, 1yr) | P1 | ✅ Done |
| FR-3.4 | Roadmaps shall include milestones and progress tracking | P1 | 🔄 In Progress |
| FR-3.5 | System shall regenerate roadmaps on demand | P1 | ✅ Done |

### FR-4: AI-Powered Course Generation
| ID | Requirement | Priority | Status |
|----|-------------|----------|--------|
| FR-4.1 | System shall generate custom learning modules for each roadmap step | P0 | ✅ Done |
| FR-4.2 | Courses shall include curated YouTube content | P0 | ✅ Done |
| FR-4.3 | System shall provide hands-on coding environments | P1 | 🔄 In Progress |
| FR-4.4 | Courses shall include quizzes and knowledge checkpoints | P1 | 🔄 In Progress |
| FR-4.5 | System shall track learning progress and completion | P0 | ✅ Done |
| FR-4.6 | Users shall receive certificates upon course completion | P2 | 📋 Planned |

### FR-5: Resume Builder & Optimizer
| ID | Requirement | Priority | Status |
|----|-------------|----------|--------|
| FR-5.1 | System shall provide structured resume creation workflow | P0 | ✅ Done |
| FR-5.2 | System shall support multiple resume templates | P0 | ✅ Done |
| FR-5.3 | System shall generate JD-specific resume optimizations | P0 | ✅ Done |
| FR-5.4 | System shall auto-update resumes as skills improve | P1 | 🔄 In Progress |
| FR-5.5 | System shall export resumes to PDF | P0 | ✅ Done |
| FR-5.6 | System shall provide ATS compatibility scores | P0 | ✅ Done |

### FR-6: AI Mock Interviews
| ID | Requirement | Priority | Status |
|----|-------------|----------|--------|
| FR-6.1 | System shall generate interview questions from resume + JD | P0 | ✅ Done |
| FR-6.2 | System shall support voice-based interview interactions | P0 | ✅ Done |
| FR-6.3 | System shall provide real-time video interview simulation (Tavus) | P0 | ✅ Done |
| FR-6.4 | System shall evaluate content, clarity, confidence, and delivery | P0 | ✅ Done |
| FR-6.5 | System shall provide actionable post-interview feedback | P0 | ✅ Done |
| FR-6.6 | System shall track interview performance history | P1 | ✅ Done |
| FR-6.7 | System shall suggest rerouting (learning) if not interview-ready | P1 | 🔄 In Progress |

### FR-7: Unified AI Career Assistant (MCP)
| ID | Requirement | Priority | Status |
|----|-------------|----------|--------|
| FR-7.1 | System shall provide a single AI assistant interface for all features | P0 | ✅ Done |
| FR-7.2 | Assistant shall maintain conversation context across sessions | P0 | ✅ Done |
| FR-7.3 | Assistant shall be able to generate courses on demand | P0 | ✅ Done |
| FR-7.4 | Assistant shall be able to initiate mock interviews | P0 | ✅ Done |
| FR-7.5 | Assistant shall provide resume feedback and fixes | P0 | ✅ Done |
| FR-7.6 | Assistant shall track and report progress | P1 | ✅ Done |

### FR-8: Job Tracking & Matching
| ID | Requirement | Priority | Status |
|----|-------------|----------|--------|
| FR-8.1 | System shall allow users to track job applications | P1 | ✅ Done |
| FR-8.2 | System shall match user profiles with job listings | P1 | 🔄 In Progress |
| FR-8.3 | System shall scrape and normalize job descriptions | P2 | 🔄 In Progress |
| FR-8.4 | System shall provide job fit scores | P2 | 📋 Planned |

### FR-9: Browser Extension
| ID | Requirement | Priority | Status |
|----|-------------|----------|--------|
| FR-9.1 | Extension shall capture job descriptions from job boards | P1 | ✅ Done |
| FR-9.2 | Extension shall provide quick ATS analysis | P1 | ✅ Done |
| FR-9.3 | Extension shall integrate with main platform seamlessly | P1 | ✅ Done |

---

## ⚙️ Non-Functional Requirements

### NFR-1: Performance
| ID | Requirement | Target | Priority |
|----|-------------|--------|----------|
| NFR-1.1 | Page load time | < 2 seconds | P0 |
| NFR-1.2 | ATS analysis completion | < 30 seconds | P0 |
| NFR-1.3 | Resume parsing | < 10 seconds | P0 |
| NFR-1.4 | API response time (p95) | < 500ms | P0 |
| NFR-1.5 | Real-time interview latency | < 300ms | P0 |

### NFR-2: Scalability
| ID | Requirement | Target | Priority |
|----|-------------|--------|----------|
| NFR-2.1 | Concurrent users | 10,000+ | P0 |
| NFR-2.2 | Background job processing | 1000 jobs/min | P1 |
| NFR-2.3 | Database connections | Auto-scaling | P0 |

### NFR-3: Reliability
| ID | Requirement | Target | Priority |
|----|-------------|--------|----------|
| NFR-3.1 | System uptime | 99.9% | P0 |
| NFR-3.2 | Data durability | 99.999% | P0 |
| NFR-3.3 | Background job retry | 3 attempts | P0 |
| NFR-3.4 | Graceful degradation | Required | P1 |

### NFR-4: Security
| ID | Requirement | Target | Priority |
|----|-------------|--------|----------|
| NFR-4.1 | Authentication | OAuth 2.0 / OIDC | P0 |
| NFR-4.2 | Data encryption at rest | AES-256 | P0 |
| NFR-4.3 | Data encryption in transit | TLS 1.3 | P0 |
| NFR-4.4 | API rate limiting | Per-user limits | P0 |
| NFR-4.5 | Resume data privacy | User-controlled | P0 |

### NFR-5: Usability
| ID | Requirement | Target | Priority |
|----|-------------|--------|----------|
| NFR-5.1 | Mobile responsiveness | Full support | P0 |
| NFR-5.2 | Accessibility | WCAG 2.1 AA | P1 |
| NFR-5.3 | Onboarding completion rate | > 80% | P1 |

---

## 📊 User Stories

### Epic 1: Career Discovery
```
US-1.1: As a student, I want to upload my resume so that the system can understand my current skills and experience.

US-1.2: As a student, I want to input my career goals so that I receive personalized guidance aligned with my aspirations.

US-1.3: As a student, I want to see a visual roadmap of my career path so that I know exactly what steps to take next.
```

### Epic 2: Learning & Upskilling
```
US-2.1: As a student, I want AI-generated courses based on my skill gaps so that I learn only what's relevant to my goals.

US-2.2: As a student, I want to track my learning progress so that I stay motivated and on schedule.

US-2.3: As a student, I want quizzes after each module so that I can validate my understanding.
```

### Epic 3: Resume Excellence
```
US-3.1: As a job seeker, I want to analyze my resume against specific job descriptions so that I can optimize my application.

US-3.2: As a job seeker, I want job-specific resume recommendations so that I improve my ATS scores.

US-3.3: As a job seeker, I want to export my optimized resume as PDF so that I can apply to jobs.
```

### Epic 4: Interview Mastery
```
US-4.1: As a job seeker, I want to practice mock interviews based on my target job so that I'm prepared for real interviews.

US-4.2: As a job seeker, I want feedback on my interview responses so that I can improve my communication.

US-4.3: As a job seeker, I want to track my interview practice history so that I can measure my improvement.
```

### Epic 5: Unified Guidance
```
US-5.1: As a student, I want a single AI assistant for all career guidance so that I don't switch between tools.

US-5.2: As a student, I want the assistant to remember my context so that I don't repeat information.

US-5.3: As a student, I want to ask natural language questions about my career so that I get personalized answers.
```

---

## 🔗 Integration Requirements

### External Services
| Service | Purpose | Priority |
|---------|---------|----------|
| **Google Vertex AI** | Multi-agent LLM orchestration | P0 |
| **OpenAI API** | Fallback LLM provider | P1 |
| **Tavus** | Video interview avatar | P0 |
| **Kinde Auth** | User authentication | P0 |
| **Inngest** | Background job processing | P0 |
| **Supabase** | Vector storage & auth | P0 |
| **Neon/PostgreSQL** | Primary database | P0 |
| **YouTube API** | Course content discovery | P1 |
| **LinkedIn** | Profile data ingestion | P2 |

### Internal APIs
| API | Purpose | Status |
|-----|---------|--------|
| tRPC Routes | Type-safe frontend-backend | ✅ Active |
| REST API (Python) | Multi-agent resume analysis | ✅ Active |
| MCP Server | AI assistant tool integration | ✅ Active |
| Inngest Functions | Event-driven background jobs | ✅ Active |

---

## 📈 Success Metrics

### Key Performance Indicators (KPIs)
| Metric | Target | Measurement |
|--------|--------|-------------|
| User Activation Rate | > 70% | Users completing onboarding |
| Resume Analysis Accuracy | > 85% | User satisfaction scores |
| Course Completion Rate | > 60% | Completed vs. started |
| Interview Improvement Score | > 30% | Score increase over sessions |
| User Retention (30-day) | > 50% | Active users returning |
| Job Placement Rate | Track | Users reporting job offers |

---

## 📅 Release Phases

### Phase 1: Foundation (MVP) ✅
- User authentication
- Resume upload & parsing
- Basic ATS analysis
- Career roadmap generation

### Phase 2: Learning Engine 🔄
- AI course generation
- YouTube content integration
- Progress tracking
- Knowledge checkpoints

### Phase 3: Interview Mastery 🔄
- Voice mock interviews
- Video avatar interviews (Tavus)
- Feedback & scoring
- Performance analytics

### Phase 4: Intelligence Layer 📋
- MCP unified assistant
- Cross-module integration
- Personalization engine
- Job matching

### Phase 5: Scale & Expand 📋
- Browser extension
- Mobile app
- B2B institutional features
- Advanced analytics

---

## 📝 Acceptance Criteria Template

Each feature must meet:
1. ✅ Functional requirements satisfied
2. ✅ Unit & integration tests passing
3. ✅ Performance benchmarks met
4. ✅ Security review completed
5. ✅ UX review approved
6. ✅ Documentation updated

---

*Document maintained by Edify-AI Engineering Team*
