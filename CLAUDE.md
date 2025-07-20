# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Codebase Overview

This appears to be an empty or newly initialized directory with no source code, configuration files, or documentation present yet. Future development work will need to establish the project structure and development workflow.

## Development Commands

No build system, package manager, or development commands have been configured yet.

## Architecture

No code architecture has been established yet.

## Session Management System (Implemented)

Complete session management library for Claude Code with context preservation and GitHub integration.

### Core Session Commands
- `/session-start [repo-name]` - Start new session (mandatory repo name)
- `/session-update [notes]` - Update session with context capture
- `/session-end` - End session with comprehensive finalization
- `/session-restore [repo-name]` - Clone previous session repository
- `/session-current` - Show active session status
- `/session-list` - List all session files
- `/session-help` - Show session help

### Session Workflow
1. **Start**: `/session-start my-project` creates GitHub repo + copies project + initializes context
2. **Update**: `/session-update` captures conversation + updates context + syncs to GitHub
3. **End**: `/session-end` creates comprehensive summary + final GitHub push with tags
4. **Restore**: `/session-restore my-project` clones previous session for continuation

### Context Management Features
- **Automatic conversation capture** in JSON format for context restoration
- **Intelligent context loading** with size estimation and recommendations
- **Progressive loading options**: Summary / Standard / Full context
- **Token estimation and management** to stay within Claude's limits
- **Security filtering** prevents sensitive data uploads to GitHub

### Repository Structure (per session)
```
[session-repo]/
├── context/
│   ├── chat-history.json      # Complete conversation for restoration
│   ├── session-notes.md       # Progress and decisions
│   ├── project-context.md     # Project structure and changes
│   ├── context-metadata.json  # Token estimates and recommendations
│   └── context-index.md       # Loading guide
├── [project-files...]         # Complete project snapshot
├── README.md                  # Session overview and continuation guide
└── metadata.json              # Session statistics and git info
```

### Key Features
- **Single-threaded sessions** (only one active at a time)
- **Mandatory GitHub backup** for all sessions
- **Context chain continuation** (clone → start new session → builds on previous)
- **Comprehensive session summaries** for future reference
- **Automatic git and project state tracking**
- **Template-based context file initialization**

## User Preferences (from ~/.claude/CLAUDE.md)

### Learning Goals
- Focus on webscraping projects and related technologies

### Development Guidelines
- Do what has been asked; nothing more, nothing less
- NEVER create files unless absolutely necessary for achieving goals
- ALWAYS prefer editing existing files to creating new ones
- NEVER proactively create documentation files (*.md) or README files unless explicitly requested