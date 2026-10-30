# Integration guidance

General guidance for contributors implementing or maintaining integrations.

## Compatibility
Document upstream ecosystem/API version, Nekomo version, Android requirements, supported features, and known limitations. Treat optional response fields as optional and expect upstream behavior to change.

## Metadata
Use stable external identifiers where available. Normalize titles carefully, retain alternate titles when possible, and do not assume every source provides complete artwork or descriptions.

## Error handling
Distinguish network errors, unavailable content, malformed responses, unsupported features, and authentication failures. Present actionable messages without exposing secrets.

## Security and privacy
Treat source responses and scripts as untrusted input. Request only necessary permissions, validate data, and avoid storing or logging credentials.

## Testing
Test successful, empty, malformed, and unavailable responses. Include device and Android-version coverage where behavior may differ.
