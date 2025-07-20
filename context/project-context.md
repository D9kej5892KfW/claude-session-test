# Project Context

## Directory Structure
```
19-07/
├── CLAUDE.md                  # Project documentation with session management system info
└── context/                   # Session context management (created during session)
    ├── chat-history.json      # Conversation capture
    ├── session-notes.md       # Progress tracking
    ├── project-context.md     # This file
    ├── context-metadata.json  # Token estimates
    └── context-index.md       # Loading guide
```

## File Summary
- **CLAUDE.md**: Project documentation including implemented session management system with context preservation and GitHub integration
- **Context files**: Complete session management structure for conversation capture and restoration

## Dependencies
- GitHub CLI (gh) for repository management
- Git for version control
- Standard shell tools (bash, find, cp, etc.)

## Configuration Files
- ~/.claude/commands/: Session management command definitions
- ~/.claude/templates/: Template files for session structure
- ~/.claude/sessions/: Local session tracking files

## Recent Changes
- Implemented complete session management library
- Created context capture and GitHub integration system
- Added conversation preservation with JSON format
- Established template-based session initialization

## Project Status
- **Total Files**: 1 (CLAUDE.md)
- **Last Modified**: 2025-07-19 23:58
- **Git Status**: Session repository created and synchronized to GitHub

## Key Components
- **Session Commands**: /session-start, /session-update, /session-end, /session-restore
- **Context Management**: Automatic conversation capture and token estimation
- **GitHub Integration**: Repository creation, synchronization, and tagging
- **Template System**: Standardized session structure with metadata tracking