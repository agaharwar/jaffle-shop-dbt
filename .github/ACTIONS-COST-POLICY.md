# Actions cost policy

Full regression and qualification workflows require a manual dispatch by the repository owner with `approved` set to true. This checkbox records approval to consume GitHub Actions minutes for that specific run; it does not replace release evidence, production approval, or any existing deployment gate.

Agents must obtain explicit user approval before dispatching an expensive run or setting this input. Ordinary requests to commit, push, or deploy are not approval for a full regression run. Automatic push, pull-request, scheduled, and deployment-event triggers must not be restored for these suites without explicit approval.

Lightweight checks may remain automatic and cancel superseded runs. Availability polling runs hourly where configured; daily backups are unchanged. Full regression remains available on demand.
