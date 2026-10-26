# Maintaining compatibility status

For every GitHub update, regenerate the compatibility table from the canonical `GolfSimHub/profiles` catalogue and explicit evidence. Do not copy a historical output table or edit a generated status only.

- Keep prepared, software-tested, practical-tested and Verified states separate.
- Record actual software test scope/date and the matching catalogue-workflow fingerprint in `release/compatibility-software-evidence.json`. A changed route must be tested again; preparation alone does not count.
- Maintain practical evidence in `GolfSimHub/profiles/compatibility-evidence.json`. A report for one connector does not transfer to another. Verified requires separate completed hardware-checklist evidence.
- Run `release/Build-CompatibilityMatrix.py --as-of YYYY-MM-DD`, the generator tests, the production compatibility test and appropriate profile round-trip tests.
- Use UTF-8. Verify rēlā and other accented text in the source, generated Markdown/JSON and the published readback.
- Sort by launch monitor/model, simulator, then connector/route. Publish the public table for the released catalogue only. Pending profiles remain in development until their beta is released.
- Publish the root table and matching machine-readable status/test-scope files together. Read them back and verify hashes, row counts and confirmed statuses.
- Documentation-only compatibility updates do not change the MSI, release version, update feed or installed configuration.
- Never upload tester contacts, private spreadsheets, keys, personal file paths or raw diagnostics as evidence. Summarise approved confirmations without identifying testers.
