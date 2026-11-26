# SoloMate - Architecture and Team Ownership

Status: DRAFT - Pending final Project Lead review
Reference date: 26 November 2026

## 1. Project Overview

SoloMate is a solo-travel assistance platform.

The application provides traveler-facing mobile
features and separate administration and service
provider web portals.

## 2. Technology Stack

### Mobile Application
- Flutter
- Dart
- Clean Architecture
- MVVM
- Domain-Driven Design principles

### Web Portals
- Angular
- TypeScript
- Feature-based architecture
- Component-Service pattern

### Backend
- ASP.NET Core .NET 8
- C#
- Layered architecture
- Repository-Service pattern
- REST API
- SignalR when approved and required

### Database
- Microsoft SQL Server
- Entity Framework Core 8
- Shared AppDbContext
- Controlled EF Core migrations

## 3. Platform Roles

### Traveler
Uses the Flutter mobile application.

### System Administrator
Uses the Angular administration portal.

### Service Provider
Uses the Angular service provider portal.

No Traveler web portal is currently approved.

## 4. Backend Architecture Rules

- Controllers handle HTTP responsibilities.
- Services contain business logic.
- Repositories handle persistence.
- Interfaces define contracts.
- DTOs define API request and response contracts.
- Models represent database entities.
- Dependency injection is required.
- Authentication, authorization and validation
  must be enforced on the backend.
- Shared database changes require lead approval.

## 5. Approved Development Modules

- Authentication
- Home
- Profile and Settings
- Trip Planning
- Connect Me / SoloConnect
- HelpMe
- Permissions and Notifications
- System Administration
- Service Provider Portal

Safety Guardian and WildGuard work is tracked
within the applicable approved project scope.

## 6. Team Responsibilities

Module ownership is maintained in the internal
Master Project Tracker.

- Project Lead: Architecture, database governance,
  integration and final acceptance.
- Trip Planning: Trip planning functionality.
- Connect Me and Notifications: Traveler connections,
  permissions and notification integrations.
- Authentication and HelpMe: Identity, authentication
  and traveler assistance workflows.
- Home and Profile: Home, Profile and Settings.
- System Administration: Angular administration portal
  and assigned safety functionality.
- Service Provider: Angular service provider portal.

Current individual assignments are maintained
in the authorized internal project tracker.


## 7. Google Maps Integration Policy

Google Maps, Routes, Places and Geocoding APIs
are not approved for current integration.

Do not introduce API keys, billing activation,
new Google Maps dependencies or external route calls.

Latitude and longitude may be stored.

Haversine distance may be used as an estimated
straight-line distance, never as road distance.

Future integration requires separate approval.

## 8. Git and Integration Rules

- Work in approved feature branches.
- Do not push directly to main or develop.
- Follow the approved Pull Request process.
- Do not merge without Project Lead authorization.
- Preserve shared contracts and security policies.
- Do not introduce unapproved dependencies.
- Verify builds and relevant regressions.

## 9. Integration Acceptance

Module completion does not automatically establish
final integrated acceptance.

Final acceptance requires applicable:
- Source compatibility review
- Security and authorization verification
- Release build verification
- Regression verification
- Database safety verification
- Project Lead approval

## 10. Documentation Policy

This is a documentation draft.

Historical evidence must be distinguished from
currently accepted integration evidence.

Do not publish credentials, raw internal source
snapshots, private database backups or personal data.

Final publication requires review and approval.