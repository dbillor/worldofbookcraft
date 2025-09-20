# Baby Book Generator Roadmap

## Product & Experience
- Clarify core flows: theme input, optional character uploads/prompts, story preview, regeneration controls
- Define 8-bit dashboard UX, prompt forms, loading animations, page flip interactions
- Detail generated book spec: up to 30 pages, per-page text + image prompt + metadata
- Plan continuity cues (character bios, color palettes, style tags) passed to both story and image models
- Determine saved book features: listing, editing metadata, re-generation, download/export

## Technical Architecture
- Choose stack (Next.js/React + Node backend) with API routes for AI orchestration
- Define data schema for books, pages, characters, assets; select storage (filesystem or DB)
- Specify orchestration pipeline: LLM prompt templates, message passing, error handling, retries
- Plan Nanobanana image API integration with seed/style persistence for continuity
- Establish media processing/storage pipeline (temporary vs permanent, CDN hooks)

## Implementation Tasks
- Scaffold project structure, package manager, lint/test tooling
- Build shared UI components (8-bit palette, dash layout, loading animations, page viewer)
- Implement forms for story intent, character uploads, advanced options
- Create backend endpoints/services for story generation, image prompts, generation queueing
- Add job tracking & status polling for page-by-page progress visualization
- Persist generated books and support retrieval and playback animation
- Implement authentication or user identity (optional placeholder)
- Instrument logging, monitoring, and error surfaces in UI

## Testing & Ops
- Create integration tests/mocks for AI + image services
- Add unit tests for pipeline logic, prompt builders, state machines
- Provide local dev fixtures and seeding scripts for sample books
- Define deployment target (Vercel/Render/etc) and CI pipeline
- Document environment variables, runbooks, and future improvements

