
---

### Sustainapi-manager (Shared libraries, schemas, build tools)

```md
# SustainAPI manager

SustainAPI manager contains shared libraries, schemas, and build tools used across all
SustainAPI repositories. It acts as the backbone for common functionality between the core blockchain, API, SDK, and smart contracts.

## Features
- Shared data models and schemas.
- Build tools and common utilities.
- Utility functions for sustainability tracking.

## Getting Started

1. fork the repository:

```json
git clone https://github.com/sustainapi/sustainapi-manager.git
```

```
cd sustainapi-manager
```

2. Install dependencies (depending on the stack you're working on):

Python:

```
pip install -r requirements.txt
```

Rust:

```
cargo build
```

TypeScript:

```
npm install
```

## Contributing
- Make sure any changes are backward-compatible with `sustainapi-rust`, `sustainapi-fastapi`,
`sustainapi-typescript`, and `sustainapi-solidity`.
- Any new features should include tests to ensure cross-repo compatibility.
## Workflow
- CI pipelines across dependent repositories will pull the latest changes from this repository.
- Versioning must be maintained to prevent breaking changes across repos.
