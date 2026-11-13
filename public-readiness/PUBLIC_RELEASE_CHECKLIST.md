# Public Release Checklist

Before copying this package into the public validation repository:

- Confirm the aggregate figures still match the final internal audit.
- Confirm no additional internal files are staged with the public commit.
- Review `git diff --cached` before pushing.
- Confirm no source code, architecture diagrams, secrets, private keys, internal vulnerability details, supplier details, personnel data or confidential remediation notes are present.
- Keep the external-assurance disclaimer intact.
- Recompute `PUBLIC_READINESS_SHA256SUMS.txt` if any public file is edited.
