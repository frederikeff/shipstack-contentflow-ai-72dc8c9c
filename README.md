# ContentFlow AI

AI-powered multi-channel content distribution platform that automatically transforms your content into platform-optimized posts across all social networks

## Project Vision

I want to build a Content Management App - I want to connect to my posts in Supabase from another application CMS style app and my Github want to stream that data into my application o a regular basis and then whenever new data is incoming, then transform that data, save it in our own database (if needed) and create ready made posts in various forms (various sizes, various kind of posts and various target groups) and then be able to decide to which platform to send them out to and when. But all automated. So basically - i.e. I get information about a new tool that I pushed to my CMS system, then we catch that data, then we create that data in forms of instagram size, linkedin size, twitter size, substack size + create text, images in various formats, workflow images and short videos (based on the tools and AI Agents we give our tool) and then we push arious formats of these content mixes out to these social media platforms where we can add new ones as needed, as well that we can add new connectors where we connect data from for the app and then we push it out based on some base rules that the user sets first (of how often to push to these systems, when to post and how often the same post after each other) and then we put that system under a stress test to make sure it works and then I want to launch that app as a multi-user SaaS platform where I price users for the usage in a freemium model, so with auth, built for scalability and built super robust, and AI-native, using MCP servers where possible and to stack that together, we can use Claude, Gemini AI, Deepseek, OpenAI and other AI tools. Let's go 

## Tech Stack

**Frontend**: Next.js 14 + TypeScript + Tailwind CSS + shadcn/ui + React Query + Zustand + Socket.io-client
**Backend**: Node.js + NestJS + PostgreSQL + BullMQ + Redis + Socket.io + Prisma ORM + Python Microservices (FastAPI) for AI/ML operations
**Deployment**: railway

## Features

1. **Multi-Source Data Connectors** - Webhook receivers and polling mechanisms to ingest content from Supabase (real-time subscriptions), GitHub (webhooks for repo changes), and extensible connector framework for adding new sources with custom parsers
2. **Content Transformation Pipeline** - Distributed job queue that processes incoming content through AI transformation chains: text optimization per platform (character limits, tone), image generation/resizing (Instagram 1:1, LinkedIn 1200x627, Twitter 1200x675), workflow diagram generation, and short-form video creation using multiple AI providers with fallback logic
3. **AI Provider Orchestration** - Unified interface managing Claude (via MCP), Gemini, DeepSeek, OpenAI, and Anthropic with intelligent routing based on task type, cost optimization, rate limiting, and automatic failover. Implements MCP (Model Context Protocol) servers for standardized AI tool interactions
4. **Platform-Specific Content Adapters** - Transform raw content into platform-optimized formats: Instagram (carousel, reels, stories), LinkedIn (articles, posts), Twitter/X (threads, single posts), Substack (newsletter formatting, HTML emails), with extensible plugin system for new platforms
5. **Multi-Platform Publishing Engine** - API integrations with social platforms (Instagram Graph API, LinkedIn API, Twitter API v2, Substack API) with OAuth2 flows, scheduling system respecting platform rate limits, automatic retry with exponential backoff, and publishing status tracking
6. **Smart Scheduling System** - User-defined posting rules (frequency per platform, time windows, timezone handling, content rotation logic to prevent duplicate consecutive posts), intelligent queue management preventing spam patterns, and A/B testing scheduler for optimal engagement times
7. **Content Preview & Approval Workflow** - Real-time preview of AI-generated content across all platforms before publishing, side-by-side comparison view, manual edit capability with version control, bulk approval/rejection, and automated approval rules based on confidence scores
8. **User Transformation Rules Engine** - Visual rule builder allowing users to define custom transformation logic (if source=GitHub then create code snippet images, if topic=AI then use technical tone), template system for reusable content patterns, and conditional publishing rules per platform
9. **Usage Tracking & Freemium Metering** - Track API calls to AI providers, social media posts published, storage used, and processing time. Implement tier-based limits (free: 10 posts/month, pro: 100 posts/month, enterprise: unlimited) with soft/hard caps and usage notifications
10. **Authentication & Multi-Tenancy** - JWT-based auth with refresh tokens, OAuth2 social login (Google, GitHub), row-level security in PostgreSQL for data isolation, workspace/team management with role-based access control (admin, editor, viewer), and API key management for external integrations
11. **Subscription & Billing Management** - Stripe integration for subscription management (freemium tiers, monthly/annual billing), usage-based overage charges, invoice generation, payment method management, dunning logic for failed payments, and upgrade/downgrade flows with prorated billing
12. **Real-Time Dashboard & Analytics** - Live job queue monitoring with Socket.io, content transformation progress bars, publishing success/failure rates per platform, engagement metrics aggregation from social APIs, cost analysis per AI provider, and visual workflow status indicators
13. **MCP Server Implementation** - Build custom MCP servers for standardized AI tool access: content analyzer MCP, image generator MCP, video processor MCP, allowing Claude and compatible AI models to use tools via Model Context Protocol specification for consistent AI agent behavior
14. **Content Version Control & History** - Store all content versions (original, transformed, published), track changes with timestamps and AI model used, enable rollback to previous versions, A/B test results storage, and audit log of all system actions for compliance
15. **Extensible Connector Framework** - Plugin architecture allowing users/developers to add custom data sources (RSS feeds, WordPress, Notion, etc.) via standardized connector interface with webhook handlers, polling configs, and data normalization schemas
16. **Load Testing & Monitoring Suite** - Built-in stress testing tools simulating high-volume content ingestion, distributed tracing with OpenTelemetry, error tracking with Sentry, performance monitoring, rate limit testing for social APIs, and automated alerting for system degradation
17. **AI Cost Optimization Engine** - Analyze cost per transformation, automatically route tasks to cheapest provider meeting quality thresholds, cache similar transformations, batch processing for efficiency, and user-facing cost estimator before approving content generation
18. **Content Queue Management** - Prioritization system for urgent vs scheduled content, manual queue reordering, pause/resume publishing per platform, emergency stop functionality, and queue health monitoring with retry policies for failed jobs

## Status

This project is being built automatically by [ShipStack](https://shipstack.ai) AI agents.

- Jules: Building features
- Claude Code / Cursor: Testing and refining

---

Built with ShipStack 🚀
