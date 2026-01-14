# Performance Checklist

- [ ] No unbounded loops over user-controlled input
- [ ] No O(n²) or worse algorithms without justification
- [ ] Expensive operations are documented (DB queries, network calls)
- [ ] Hot paths are identified and kept simple
- [ ] Caching decisions are explicit (or explicitly deferred)
- [ ] No polling or busy-wait loops
- [ ] Timeouts are set on external calls
- [ ] Performance tradeoffs are documented if knowingly accepted
