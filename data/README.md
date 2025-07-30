# BabyCoach Data Directory

This directory contains data files and symbolic links to external data sources.

## Security Notice
- **NO personal data should ever be committed to git**
- Personal note corpus is accessed via symbolic link to external location
- All `.json`, `.db`, and personal data files are excluded in `.gitignore`

## Structure
- `corpus/` - Symbolic link to your Evernote export JSON
- `vector_store/` - Local vector database storage (excluded from git)
- `exports/` - Any data exports or backups (excluded from git)

## Setup
The corpus data is accessed via symbolic link:
```bash
ln -s ~/Desktop/evernote_rag_export_*.json data/corpus.json
```

This ensures your personal notes never accidentally get committed while maintaining easy access for development.
