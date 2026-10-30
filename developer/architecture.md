# Architecture overview

This document describes conceptual boundaries and is not a substitute for the current source code.

A maintainable client benefits from separating:
- **Presentation:** screens, navigation, accessibility, and device-specific layouts.
- **Catalogue and metadata:** title identity, descriptions, artwork, and lookup.
- **Source integration:** discovery and communication with supported external ecosystems.
- **Content resolution:** retrieving streams or chapter content from a selected source.
- **Tracking:** synchronization with supported third-party providers.
- **Settings and persistence:** user preferences, source configuration, and local state.

Keep metadata retrieval independent from content source availability where practical. Handle optional fields and upstream failures gracefully, validate external data, and never log secrets.

For implementation details, inspect the [Nekomo source repository](https://github.com/Nekomo-App/Nekomo).
