# Integration guidance

This page provides general guidance for contributors implementing or maintaining integrations.

## Compatibility

Document the upstream ecosystem/API version, Nekomo version, Android requirements, supported features, and known limitations. Treat optional response fields as optional and expect upstream behavior to change.

## Metadata

Use stable external identifiers when available. Normalize titles and metadata carefully, retain alternate titles where possible, and avoid assuming that every source provides complete artwork or descriptions.

## Error handling

Distinguish network errors, unavailable content, malformed responses, unsupported features, and authentication failures. Present actionable messages without exposing internal secrets.

## Security and privacy

Treat source responses and scripts as untrusted input. Request only necessary permissions, validate data, and avoid storing or logging credentials unnecessarily.

## Testing

Test successful, empty, malformed, and unavailable responses. Include device and Android-version coverage where behavior may differ.
