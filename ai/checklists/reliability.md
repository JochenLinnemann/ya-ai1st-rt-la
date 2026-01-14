# Reliability Checklist

- [ ] Failure modes are identified and documented
- [ ] External dependencies have timeouts
- [ ] Retries are bounded and justified
- [ ] Errors are handled explicitly (not swallowed)
- [ ] System degrades gracefully on partial failure
- [ ] Startup and shutdown behavior is deterministic
- [ ] State is recoverable after restart
- [ ] Monitoring is updated if behavior changes

## Exceptions

If any checklist item is intentionally not met:
- Document the reason
- Document the risk
- Document the mitigation (if any)
