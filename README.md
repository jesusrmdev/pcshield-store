# PcShield Store — Helpdesk Application

A web-based helpdesk application for managing technical support tickets, built with HTML5, Tailwind CSS and Vanilla JavaScript.

**Live demo:** https://sparkly-dodol-373c21.netlify.app  
**Educational repository:** https://github.com/2416082-debug/daw2-fiag/tree/main/ut2-prompt-engineering/01-taller-helpdesk

## Project Background

PcShield Store was originally developed by me as an academic project within the **Fundamentals of Generative Artificial Intelligence (FIAG)** module of the Higher Vocational Training programme in Web Application Development (2º DAW), during the 2026–2027 academic year at IES Alcántara.

The project was developed as part of the coursework on prompt engineering, AI-assisted development, reusable Skills and formal software specification using OpenSpec.

This repository contains the academic version of the project, developed and documented as part of the UT2 workshop. The project may also be presented in a separate professional GitHub repository as part of my developer portfolio.

## Overview

PcShield Store simulates a helpdesk environment for managing technical support incidents in an online computer store.

It provides an interactive dashboard and a ticket-management workflow that allows users to create, view, search, filter, resolve and delete support tickets.

The application also includes a security-focused area for demonstrating the detection and anonymisation of personal data, as well as protection mechanisms against potentially dangerous HTML/JavaScript content and prompt injection attempts.

## Main Features

- **Interactive dashboard:** KPI cards and statistics summarising support tickets.
- **Ticket management:** Create, view, resolve and delete incidents.
- **Search and filtering:** Find tickets using keywords and categories.
- **Initial data loading:** Sample tickets loaded from `datos_tickets.json`.
- **Local persistence:** Ticket changes stored in the browser using `localStorage`.
- **Personal data protection:** Detection and anonymisation of DNI/NIE numbers, payment-card numbers and IPv4 addresses.
- **XSS protection:** Detection and blocking of potentially dangerous HTML and JavaScript content.
- **Prompt Injection detection:** Identification and blocking of suspicious instructions.
- **RGPD Testing Laboratory:** Interactive tests for personal-data anonymisation and prompt injection detection.
- **Dynamic statistics:** Visual representation of incidents by category.

## Technology Stack

- **HTML5** — Application structure and semantic markup.
- **Tailwind CSS** — Interface styling and responsive design.
- **Vanilla JavaScript** — Application logic and interactive functionality.
- **JSON** — Initial sample ticket data.
- **localStorage** — Client-side data persistence.
- **OpenCode** — AI-assisted development environment.
- **Prompt Engineering** — Structured instructions and reusable commands.
- **Skills** — Reusable instructions for web design and RGPD-related protection.
- **OpenSpec** — Formal specification and task planning.
- **Git and GitHub** — Version control and source-code hosting.
- **Netlify** — Application deployment.

## Development Workflow

The application was developed through a structured AI-assisted workflow rather than relying on unplanned code generation.

The main stages included:

1. Defining the project context and technical rules in `AGENTS.md`.
2. Creating a custom OpenCode command to anonymise and classify incoming support messages.
3. Installing the official `web-design-guidelines` Skill and creating a custom `escudo-rgpd-js` Skill.
4. Defining application requirements and implementation tasks using OpenSpec.
5. Building the application through a three-stage Prompt Chaining process.
6. Auditing and improving the application using the Reflection pattern.
7. Designing and implementing an individual RGPD Testing Laboratory through a new OpenSpec change.
8. Testing the application and deploying it using Netlify.

## Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/2416082-debug/daw2-fiag.git
   ```

2. Open the project folder:

   ```bash
   cd daw2-fiag/ut2-prompt-engineering/01-taller-helpdesk
   ```

3. Open the folder in Visual Studio Code.

4. Start the application using the Live Server extension or another local static web server.

5. Open the local URL provided by the server.

No backend installation or database configuration is required.

## Data and Technical Scope

The application loads its initial sample tickets from `datos_tickets.json` and stores subsequent changes in the browser's `localStorage`.

Ticket modifications are local to the browser and origin where the application is running. They are not synchronised between devices and do not modify the original JSON file in the repository.

PcShield Store is a frontend demonstration. It does not currently provide a production backend, shared multi-user storage, a remote database or live AI integration.

The privacy and security mechanisms are educational demonstrations. They should not be considered a substitute for server-side validation, production security controls or a formal GDPR compliance assessment.

## Project Purpose

This project demonstrates practical experience with frontend development, client-side data management, helpdesk workflows, AI-assisted software development and security-aware interface design.

It also documents the application of prompt engineering, reusable Skills, formal specifications and iterative auditing within a real development workflow.

## Author

**Jesús Rodríguez Marín**

GitHub: [@2416082-debug](https://github.com/2416082-debug)

---

*Originally developed as an academic project for the FIAG module at IES Alcántara (2026–2027).* 