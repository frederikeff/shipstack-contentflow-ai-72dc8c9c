# Agent Instructions

This repository is being built by AI agents. Follow these guidelines:

## Architecture

**Frontend**: Next.js 14 + TypeScript + Tailwind CSS + shadcn/ui + React Query + Zustand + Socket.io-client
**Backend**: Node.js + NestJS + PostgreSQL + BullMQ + Redis + Socket.io + Prisma ORM + Python Microservices (FastAPI) for AI/ML operations
**Database**: PostgreSQL (Railway)

## Project Structure

```
/
├── frontend/       # Next.js 14 + TypeScript + Tailwind CSS + shadcn/ui + React Query + Zustand + Socket.io-client
├── backend/        # Node.js + NestJS + PostgreSQL + BullMQ + Redis + Socket.io + Prisma ORM + Python Microservices (FastAPI) for AI/ML operations
├── README.md       # Project documentation
└── AGENTS.md       # This file
```

## Development Guidelines

### Code Quality
- Write clean, idiomatic code for the chosen language
- Include TypeScript types (if applicable)
- Add error handling for all operations
- Write comments for complex logic
- Follow best practices for the framework

### Testing
- Write unit tests for business logic
- Write integration tests for API endpoints
- Ensure all tests pass before merging
- Test error scenarios

### Git Workflow
1. Create feature branch: `feature/feature-name`
2. Implement feature with tests
3. Commit with clear messages
4. Push to branch
5. AI will test and merge to main

### API Guidelines
- RESTful endpoints
- Proper HTTP status codes
- JSON responses
- Error responses with helpful messages
- Input validation

### Database
- Use migrations for schema changes
- Index frequently queried fields
- Use foreign keys for relationships
- Validate data before saving

## Vision

Dashboard for content monitoring, AI-generated preview management, scheduling calendar, platform connection management, and analytics visualization with real-time status updates

Orchestrates data ingestion from multiple sources (Supabase, GitHub), manages AI transformation pipelines using multiple LLM providers, handles job queuing for content generation, executes MCP server protocols, manages multi-platform publishing APIs, and provides usage tracking for billing

## Requirements

- User authentication required
- Multi-user support required
- Stripe payment integration required
- External APIs: Supabase Realtime API, GitHub Webhooks API, Instagram Graph API, LinkedIn API, Twitter API v2, Substack API, OpenAI API, Anthropic Claude API, Google Gemini API, DeepSeek API, Stripe API, AWS S3 (media storage), Cloudflare R2 (alternative storage)

## Deployment

This project will be automatically deployed to Railway when merged to main.

---

*This file is used by AI agents to understand the project architecture and coding standards.*
