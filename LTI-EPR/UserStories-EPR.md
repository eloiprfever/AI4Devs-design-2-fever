# User Stories

## User Story 1: Centralized Applicant Management
**Title:** As a recruiter, I want to manage all applicant information in a centralized dashboard so that I can efficiently track and process candidates through the hiring pipeline.

**Description:**
The system should provide a comprehensive dashboard where recruiters can view, organize, and manage all applicant information. This includes parsed resume data, application status, and communication history. The dashboard should allow real-time updates and provide clear visibility of the candidate's progress through different hiring stages.

**Acceptance Criteria:**
- Dashboard displays a list of all active applications with key information
- Ability to view detailed applicant profiles with parsed resume data
- Real-time status updates for each candidate in the hiring pipeline
- Search and filter capabilities by various criteria (status, position, date)
- Option to add notes and update candidate status
- Collaboration features for sharing candidate information with team members
- Export functionality for candidate data and reports

**Story Points:** 13

## User Story 2: AI-Powered Candidate Screening
**Title:** As a hiring manager, I want the system to automatically screen and rank candidates using AI so that I can quickly identify the most qualified applicants.

**Description:**
The system should use AI algorithms to analyze candidate applications, compare them against job requirements, and provide a ranked list of candidates. This should include automatic parsing of resumes and scoring based on predefined criteria.

**Acceptance Criteria:**
- AI engine automatically parses and analyzes incoming applications
- Candidates are automatically ranked based on job requirements match
- Clear scoring system with explanation of ranking criteria
- Ability to customize ranking parameters per position
- Highlight key qualifications and skills matches
- Flag potential concerns or missing requirements
- Option to override AI rankings with manual adjustments

**Story Points:** 8

## User Story 3: Intelligent Decision Support
**Title:** As a recruiter, I want AI-assisted insights during the hiring decision process so that I can make more objective and data-driven hiring decisions.

**Description:**
The system should analyze interview feedback, candidate assessments, and historical hiring data to provide intelligent recommendations for hiring decisions, helping reduce bias and improve hiring accuracy.

**Acceptance Criteria:**
- Collect and aggregate feedback from all interviewers
- Generate AI-powered hiring recommendations based on all available data
- Provide bias detection and warnings
- Compare candidates against successful past hires
- Display decision-supporting metrics and insights
- Generate comprehensive candidate evaluation reports
- Allow configuration of decision criteria weights

**Story Points:** 5

# Backlog

## Priority 1 - MVP Foundation
### US1: Centralized Applicant Management (13 SP)
- Highest business value: Core functionality needed for basic ATS operations
- Required foundation for other features
- Dependencies: None
- Key for MVP: Basic applicant tracking is essential for minimal viable product
- Implementation complexity: High due to database and UI requirements

## Priority 2 - Enhanced Screening
### US2: AI-Powered Candidate Screening (8 SP)
- High business value: Major differentiator from traditional ATS
- Dependencies: Requires US1 to be implemented first
- Medium complexity: Can be implemented incrementally
- MVP Enhancement: Can start with basic screening algorithms and improve over time

## Priority 3 - Advanced Features
### US3: Intelligent Decision Support (5 SP)
- Medium business value: Nice to have but not essential for MVP
- Dependencies: Requires both US1 and US2
- Lower complexity but needs data from previous features
- Post-MVP: Can be added once core functionality is stable


| Priority | User Story | Story Points |
|----------|------------|--------------|
| 1 | As a recruiter, I want to manage all applicant information in a centralized dashboard | 13 |
| 2 | As a hiring manager, I want the system to automatically screen and rank candidates using AI | 8 |
| 3 | As a recruiter, I want AI-assisted insights during the hiring decision process | 5 |

**Total Story Points:** 26

# Technical Tickets for AI-Powered Candidate Screening

## Ticket 1: Resume Parser Implementation
**Title:** Implement AI-based Resume Parser Engine

**Description:**  
Develop a machine learning model and API endpoint to automatically extract and structure information from resumes in various formats (PDF, DOC, DOCX).

**Acceptance Criteria:**
- Support for multiple file formats (PDF, DOC, DOCX)
- Extract key information: contact details, work experience, education, skills
- 90% accuracy in data extraction
- API endpoint for resume upload and parsing
- Error handling for unsupported formats or corrupted files
- Structured JSON output format

**Priority:** High  
**Story Points:** 5  
**Assignee Team:** ML/AI Team

## Ticket 2: Candidate Ranking System
**Title:** Create AI Ranking Algorithm for Candidates

**Description:**  
Develop an algorithm to compare parsed resume data against job requirements and generate a ranking score for each candidate.

**Acceptance Criteria:**
- Configurable weighting system for different criteria
- Score calculation based on skills match
- Experience relevancy assessment
- Education requirements matching
- Generate detailed scoring breakdown
- API endpoint for ranking requests
- Unit tests with 95% coverage

**Priority:** High  
**Story Points:** 5  
**Assignee Team:** ML/AI Team

## Ticket 3: Ranking UI Implementation
**Title:** Develop Ranking Dashboard Interface

**Description:**  
Create a user interface to display candidate rankings and allow customization of ranking parameters.

**Acceptance Criteria:**
- Display ranked list of candidates with scores
- Interactive filters and sorting options
- Parameter customization interface
- Score breakdown visualization
- Mobile-responsive design
- Accessibility compliance (WCAG 2.1)

**Priority:** Medium  
**Story Points:** 3  
**Assignee Team:** Frontend Team

## Ticket 4: Job Requirements Matcher
**Title:** Implement Job Requirements Matching System

**Description:**  
Create a system to analyze job descriptions and match them against candidate profiles.

**Acceptance Criteria:**
- Job requirements parser
- Skills keyword extraction
- Experience level matching
- Required vs preferred criteria handling
- Match percentage calculation
- API endpoint for requirements matching

**Priority:** Medium  
**Story Points:** 3  
**Assignee Team:** Backend Team

## Ticket 5: Integration and Testing
**Title:** System Integration and E2E Testing

**Description:**  
Integrate all components and perform end-to-end testing of the candidate screening system.

**Acceptance Criteria:**
- Integration tests for all components
- End-to-end workflow testing
- Performance testing under load
- Error handling verification
- Security testing completion
- Documentation of all APIs and interfaces

**Priority:** High  
**Story Points:** 2  
**Assignee Team:** QA Team

