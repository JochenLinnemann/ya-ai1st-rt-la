# Security Checklist

This checklist applies to both human- and AI-generated changes.
Each item should be answerable with a clear yes/no.

## Input & Data Handling
- [ ] All external input is validated or sanitized
- [ ] No trust is placed in client-provided data
- [ ] Input size limits are enforced where applicable
- [ ] Dangerous formats (e.g. raw SQL, shell input) are not accepted unchecked

## Authentication & Authorization
- [ ] Authentication logic is explicit and centralized
- [ ] Authorization checks exist for protected actions
- [ ] Privilege levels are minimal and intentional
- [ ] No authorization decisions are implied or indirect

## Secrets & Sensitive Data
- [ ] No secrets, tokens, or credentials are hardcoded
- [ ] Secrets are not logged or returned in errors
- [ ] Configuration handling avoids accidental leakage
- [ ] Sensitive data is masked or redacted where appropriate

## Dependencies & Supply Chain
- [ ] New dependencies are justified
- [ ] Dependency versions are pinned or constrained
- [ ] No abandoned or unmaintained dependencies introduced
- [ ] Transitive dependency risk is considered for critical paths

## Error Handling & Observability
- [ ] Errors do not expose internal implementation details
- [ ] Stack traces are not exposed to end users
- [ ] Security-relevant failures are logged appropriately
- [ ] Logs do not contain sensitive data

## AI-Specific Security Considerations
- [ ] AI did not generate authentication or crypto logic without review
- [ ] AI-generated code was reviewed for injection vulnerabilities
- [ ] AI suggestions introducing dynamic code execution were rejected or scrutinized
- [ ] AI was not used to generate secrets or credentials

## Operational Security
- [ ] Security impact of the change is understood
- [ ] New attack surfaces are documented
- [ ] Rollback does not weaken security controls
- [ ] Monitoring or alerts updated if risk profile changes
