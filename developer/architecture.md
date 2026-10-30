# Architecture overview

This document describes conceptual boundaries for Nekomo. It is not a substitute for the current source code.

A maintainable client benefits from separating these responsibilities:

- **Presentation:** screens, navigation, accessibility, and device-specific layouts.
- **Catalogue and metadata:** title identity, descriptions, artwork, and catalogue lookup.
- **Source integration:** discovery and communication with supported external source ecosystems.
- **Content resolution:** retrieving streams or chapter content from a selected source.
- **Tracking:** synchronization with supported third-party tracking providers.
- **Settings and persistence:** user preferences, source configuration, and local state.

## Design principles

- Keep metadata retrieval independent from content source availability where practical.
- Handle missing optional fields and upstream failures gracefully.
- Avoid coupling UI components directly to individual providers.
- Validate external data before displaying or processing it.
- Do not log secrets or private account data.
- Document format and API compatibility explicitly.

For implementation details, inspect the current [Nekomo source repository](https://github.com/Nekomo-App/Nekomo).
