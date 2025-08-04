# pawd

**A modern .NET-based platform for connecting pet enthusiasts, professionals, and creators.**

---

## Overview

**pawd** is an open source ecosystem designed to bring together pet owners, service providers, and community creators through a modular, extensible suite of services. Whether it’s booking a pet photographer, finding a vet, or sharing adorable pet moments, pawd provides the foundation for a connected pet community—all built on modern .NET technologies.

---

## Architecture

The pawd ecosystem follows clean, modular design principles and is composed of several independently developed services:

### 🟢 Auth Service (`pawd.Auth`)
- Provides secure user authentication and authorization across the pawd ecosystem
- Implements OAuth2 flows (password and authorization code grants) using OpenIddict
- Built for easy integration with other pawd services

### 🟢 API Service (`pawd.API`)
- The core REST API for business logic and user-facing operations
- Implements Clean Architecture (Domain, Application, Infrastructure, API)
- CQRS with MediatR, ASP.NET Core Identity, Entity Framework Core (SQL Server)
- Integrates custom authentication and image processing

### 🟢 Image Processing & Job Workers (`pawd.ImageProcessing`, Job Management)
- Handles background image processing, storage, and other asynchronous tasks
- Includes a flexible job management SDK for queuing, status tracking, and retries
- Extensible to support additional job types and messaging systems

### 🟢 Core Library (`pawd.CoreLibrary`)
- Shared utilities and building blocks for the ecosystem
- Features a fluent, strongly-typed HAL-FORMS builder for dynamic API forms
- Plans for extensible logging and additional shared functionality

---

## Current Status

pawd is actively in development, with all major services evolving rapidly.  
APIs, SDKs, and internal structures may change frequently as the platform matures.

---

## Project Goals

- Provide a secure, extensible foundation for pet-focused applications
- Enable seamless integration of authentication, business logic, and background processing
- Promote clean architecture and maintainable code across all services
- Make it easy for contributors and recruiters to explore modern .NET patterns in practice

---

## Ecosystem Summary

| Service              | Purpose                                                   | Technology           |
|----------------------|-----------------------------------------------------------|----------------------|
| Auth                 | Authentication & Authorization (OAuth2)                   | .NET 8, OpenIddict   |
| API                  | Core Business Logic & REST API                            | .NET 8, MediatR, EF  |
| ImageProcessing/Jobs | Background Processing & Job Management                    | .NET 8, SDK          |
| Core Library         | Shared Tools (e.g., HAL-FORMS, Logging)                   | .NET 8               |

---

**For service-specific documentation, see the individual project directories.**

---

