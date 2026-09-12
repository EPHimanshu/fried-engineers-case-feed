# Fried Engineers Case Feed

Public, read-only deployment feed for Fried Engineers Case Files.

This repository intentionally contains **publishable case payloads only**. The private factory, prompts, validators, backlog, automation logic and authoring system stay in the private `fried-engineers-case-files` repository.

WordPress reads `manifest.json`, fetches the listed case JSON files, verifies their SHA-256 hashes, and creates or updates Case File posts.

Publishing rule:
- `approved` → WordPress draft
- `published` → WordPress live post

Do not commit secrets, credentials, private prompts, or internal planning data here.
