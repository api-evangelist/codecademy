# Codecademy GraphQL Schema

## Overview

This GraphQL schema represents a conceptual model of the Codecademy online programming education platform. Codecademy provides interactive coding tutorials, career paths, certifications, and bootcamps across programming languages, data science, AI, cloud computing, cybersecurity, and web development.

The schema covers the core domain objects of the Codecademy platform, based on its partner API documentation at https://partners.codecademy.com/api/documentation and the public platform structure visible at https://www.codecademy.com.

## Schema Source

- **Schema File**: [codecademy-schema.graphql](codecademy-schema.graphql)
- **Partner API Docs**: https://partners.codecademy.com/api/documentation
- **Platform**: https://www.codecademy.com
- **Parent Company**: https://www.skillsoft.com

## Domain Coverage

The schema covers the following domains:

### Learner Domain
Types covering learner identity, profiles, skills, and progress tracking across the platform. Includes `User`, `UserDetails`, `UserProfile`, `UserSkills`, `Learner`, and `LearnerDetails`.

### Content Domain
Types representing the hierarchical structure of Codecademy learning content: `Course`, `CourseDetails`, `CourseContent`, `Track`, `TrackDetails`, `Path`, `PathDetails`, `Lesson`, `LessonDetails`, `Exercise`, `ExerciseDetails`, `ExerciseType`, `Quiz`, `QuizDetails`, `Project`, and `ProjectDetails`.

### Skills Domain
Types for the skill taxonomy and skill-based learning: `Skill`, `SkillDetails`, and `SkillSet`.

### Progress Domain
Types tracking learner progress and completions: `Progress`, `ProgressDetails`, `TrackProgress`, `PathProgress`, and `Completion`.

### Credentialing Domain
Types for certificates and certification paths earned on the platform: `Certificate`, `CertificateDetails`, and `CertificationPath`.

### Team and Organization Domain
Types for business and team-based learning management: `Team`, `TeamDetails`, `TeamMember`, `Plan`, `PlanDetails`, and `Subscription`.

### Enrollment and Assignment Domain
Types for managing learner enrollments and assignments: `Enrollment`, `EnrollmentDetails`, `Assignment`, `AssignmentDetails`, `Cohort`, and `CohortDetails`.

### Platform Domain
Types for workspaces and platform infrastructure: `Workspace` and `WorkspaceDetails`.

### API Access Domain
Types for authentication and programmatic access: `APIKey`, `Token`, and `Webhook`.

## Type Count

This schema defines 55 named types covering the full breadth of the Codecademy platform.

## Notes

Codecademy does not expose a fully public developer REST API for general consumption. The partner API at https://partners.codecademy.com/api/documentation is available to business and enterprise partners for managing team learning, enrollment, progress reporting, and content access. This GraphQL schema is a conceptual representation of the platform domain model suitable for partner integrations.
