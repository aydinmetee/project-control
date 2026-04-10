# System Design

## Overview
The system consists of three main parts:

1. project-control
   - stores product, architecture, and execution documents
   - stores issue templates
   - acts as the source of truth for planning and orchestration

2. project-backend
   - provides the backend API for todo operations
   - contains domain logic, persistence, and backend tests

3. project-frontend
   - provides the user interface for todo operations
   - consumes backend APIs
   - contains frontend UI logic and frontend tests

## High-Level Flow
1. Product requirements are defined in project-control.
2. Work is split into slices and tasks in project-control.
3. Backend and frontend tasks are created from the active slice.
4. Backend and frontend repositories implement their own tasks.
5. Pull requests are reviewed and validated.
6. Human approval happens at PR stage.

## Backend Responsibilities
- Manage todo data
- Validate backend input
- Expose API endpoints
- Persist todo state
- Return consistent responses

## Frontend Responsibilities
- Show todo list
- Allow todo creation
- Allow marking todo as completed
- Show validation and error states
- Communicate with backend API

## Control Repository Responsibilities
- Keep source-of-truth documents
- Store slice planning
- Store issue templates
- Track execution state

## Initial Domain Model
Todo:
- id
- title
- completed
- visible

## Initial Core Flow
1. User opens todo screen
2. User sees existing todos
3. User creates a new todo
4. User marks a todo as completed
5. UI reflects the updated state

## Non-Goals for MVP
- Authentication
- Multi-user support
- Notifications
- Advanced search/filtering
- Deployment automation