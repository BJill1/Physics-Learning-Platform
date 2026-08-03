**Version:** 1.0
**Status:** Baseline (Frozen)
**Last Updated:** August 3, 2026



# Functional Requirements

**Project:** Physics Learning Platform  
**Milestone:** Milestone 1 – Physics Assessment Platform

## Purpose

This document defines the functional requirements for Milestone 1 of the Physics Learning Platform. Each requirement specifies a function that the system shall perform.

---

# 2.1 User Registration and Authentication

## Student Registration

**FR-001:** The system shall allow a student to register using a unique username and password.

**FR-002:** The system shall require the student to confirm the password during registration.

**FR-003:** The system shall allow students to optionally provide an email address and mobile phone number.

**FR-004:** The system shall prevent duplicate usernames.

**FR-005:** The system shall activate a student account immediately after successful registration.


## Teacher Registration

**FR-006:** The system shall allow a teacher to register using their full name, school name, email address, mobile phone number, and password.

**FR-007:** The system shall require the teacher to verify either the registered email address or mobile phone number.

**FR-008:** The system shall send a verification code or verification link using the teacher's selected verification method.

**FR-009:** The system shall reject expired, invalid, or previously used verification codes or links.

**FR-010:** The system shall allow teachers to request a new verification code or link.

**FR-011:** The system shall place newly registered teachers in a **Pending Verification** state.

**FR-012:** The system shall store the teacher's school information for teacher verification.

**FR-013:** Unverified teachers shall not have access to teacher-only features but shall be permitted to access student practice features.

**FR-014:** The system shall change the teacher account status to **Verified** after successful teacher verification.


## Login

**FR-015:** Students shall log in using their username and password.

**FR-016:** Teachers shall log in using their verified email address or verified mobile phone number together with their password.

**FR-017:** The system shall reject invalid login credentials.

**FR-018:** The system shall create a secure authenticated session after successful login.

**FR-019:** The system shall allow authenticated users to log out.

**FR-020:** Users with a verified email address or verified mobile phone number shall be able to reset forgotten passwords.


# 2.2 Role-Based Access Control

**FR-021:** The system shall support two user roles: Teacher and Student.

**FR-022:** Student registrations shall receive the Student role while verified teacher registrations shall receive the Teacher role.

**FR-023:** Teacher-only features shall be accessible only to verified teachers.

**FR-024:** Students shall have access to the student practice module.

**FR-025:** Verified teachers shall also have access to the student practice module.

**FR-026:** Students shall not have access to teacher-only features.

**FR-027:** Teachers and students shall have read-only access to the Physics question bank.

**FR-028:** Teachers and students shall have read-only access to the worksheet library.

**FR-029:** The system shall enforce role permissions on both the client and server.

# 2.3 Teacher Assessment Generation

**FR-030:** Verified teachers shall be able to generate Physics
assessments.

**FR-031:** Teachers shall select the educational level.

**FR-032:** The system shall display only topics belonging to the
selected educational level.

**FR-033:** Teachers shall select a Physics topic for MCQ generation and worksheet download.

**FR-034:** Teachers shall specify the required number of questions for MCQ generation.

**FR-035:** The system shall enforce a configurable maximum number of
questions.

**FR-036:** The system shall prevent requests exceeding the available
number of questions.

**FR-037:** The system shall notify the teacher when insufficient
questions exist.

**FR-038:** Questions shall be selected only from the curated Physics
question bank.

**FR-039:** Duplicate questions shall not appear within the same
assessment.

**FR-040:** The system shall generate an answer key for MCQ.

**FR-041:** Mathematical expressions, diagrams, tables, and scientific
notation shall be preserved.

**FR-042:** Teachers shall not be permitted to modify, add, remove, or
replace question-bank content.

# 2.4 Assessment Preview, Printing and Download

**FR-043:** Teachers shall preview assessments before printing or
downloading.

**FR-044:** The preview shall display questions in a printable format.

**FR-045:** Formatting, numbering, diagrams, equations, and tables shall
be preserved.

**FR-046:** Teachers shall be able to print generated assessments.

**FR-047:** Teachers shall be able to download assessments as PDF files.

**FR-048:** Teachers shall be able to print or download answer keys for MCQ.

**FR-049:** Downloaded PDFs shall preserve the preview formatting.

# 2.5 PDF Worksheet Library

**FR-050:** Verified teachers shall have access to downloadable PDF
worksheets.

**FR-051:** Worksheets shall be organized by educational level.

**FR-052:** Worksheets shall be organized by Physics topic.

**FR-053:** Each downloadable worksheet shall contain fields for:

- Student Name
- School
- Number on Class List
- Class

# 2.6 Student Practice

**FR-054:** Teachers shall be able to preview worksheets where
available.

**FR-055:** Teachers shall be able to download worksheets.

**FR-056:** The original worksheet shall remain unchanged during preview
and download.

**FR-057:** Teachers shall have read-only access to worksheets.
**FR-058:** Authenticated students shall be able to begin a practice
session.

**FR-059:** Verified teachers shall also be able to access the student
practice module.

**FR-060:** Users shall select an educational level.

**FR-061:** The system shall display topics for the selected educational
level.

**FR-062:** Users shall select a Physics topic.

**FR-063:** Questions shall be retrieved from the curated Physics
question bank.

**FR-064:** MCQ for the students shall be displayed one at a time.

**FR-065:** All answer options for MCQ for the students shall be displayed.

**FR-066:** User shall select one answer before submission.

**FR-067:** The system shall prevent blank submissions.

**FR-068:** The system shall evaluate submitted answers and provide immediate feedback after each
submitted answer.

**FR-069:** The system shall display the correct answer after an
incorrect response.

**FR-070:** Users shall be able to proceed to the next question after
receiving feedback.

**FR-071:** Duplicate questions shall not appear during a practice
session.

**FR-072:** The system shall maintain the user's score throughout the
practice session.

**FR-073:** The system shall display the number of completed questions.

**FR-074:** The system shall display the final score at the end of the
practice session.

**FR-075:** The system shall display a performance summary at the end of the practice session containing:

- Total questions attempted
- Correct answers
- Incorrect answers
- Percentage score

**FR-076:** Long-term progress tracking shall not be required in
Milestone 1.

# 2.7 Search and Navigation

**FR-077:** The system shall provide navigation appropriate to the
user's role.

**FR-078:** Teachers shall have navigation to: - Assessment Generation -
PDF Worksheet Library - Student Practice

**FR-079:** Students shall have navigation to: - Student Practice

**FR-080:** Teachers shall be able to search worksheets.

**FR-081:** Teachers shall be able to filter worksheets by educational
level and topic.

**FR-082:** The system shall allow users to return to the dashboard from
all major pages.

**FR-083:** The system shall display clear page headings and navigation
labels.

**FR-084:** The system shall display an appropriate message when no
matching content is found.

# 2.8 Feedback

**FR-085:** Authenticated teachers and students shall be able to submit
feedback.

**FR-086:** The system shall allow users to categorize feedback as: -
Bug Report - Question Error - Worksheet Error - Feature Suggestion -
General Feedback

**FR-087:** The system shall allow users to enter a textual description
of their feedback.

**FR-088:** The system shall acknowledge successful feedback submission.

**FR-089:** The system shall record the submitted feedback together
with: - User role - Username - Date and time of submission - Feedback
category

**FR-090:** Only authenticated users shall be permitted to submit
feedback.





## Revision History

| Version | Date | Description |
|----------|------|-------------|
| 1.0 | 2026-08-03 | Initial baseline for Milestone 1 Functional Requirements. |


