# Changelog

## v2.0.6

### Fixed
- TizenBrew now works on Tizen 9 and Tizen 10. The service is started through `wrt:service` on these versions, because `launchAppControl` no longer starts it there (it either failed with "Unknown error" or the UI kept reloading forever).
- After starting the service, the UI waits up to 30 seconds for it to come up instead of reloading right away.

Older Tizen versions keep using the previous launch method.
