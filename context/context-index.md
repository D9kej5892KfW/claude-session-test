# Context Loading Guide

## Available Context Files

### 📝 session-notes.md (~[tokens] tokens)
- Session progress and key decisions
- Issues and solutions
- Goals and next steps

### 🗂️ project-context.md (~[tokens] tokens)  
- Project structure and file summary
- Dependencies and configuration
- Recent changes and git status

### 💬 chat-history.json (~[tokens] tokens)
- Complete conversation history
- All user messages and Claude responses
- Full context for continuation

## Loading Recommendations

### ⚡ Quick Start (< 5k tokens)
Load only `session-notes.md` for basic context continuation.

### 🔄 Standard Load (< 20k tokens)
Load `session-notes.md` + `project-context.md` for balanced context.

### 🎯 Full Context (< 50k tokens)
Load all files for complete conversation and project awareness.

## Current Context Status
- **Total estimated tokens**: [total]
- **Recommended load**: [recommendation]
- **Last updated**: [timestamp]