# Changelog

## 0.1.2 - 2026-11-12

- `security-design-review` reads a review's gaps and records a verdict on each (accept fix, accepted risk, false positive, or reopen) with `pi_design_review_gap_update_status`, after tenant verification and explicit confirmation.

## 0.1.1 - 2026-08-25

- Bound secure-development guidance to one playbook lookup for a stable task.
- When playbook coverage is adjacent or missing, report the gap and continue from current repository evidence without retries or fallback lookups.

## 0.1.0 - 2026-08-12

Initial release of Pi Security for Cursor IDE.

- Investigate findings and review security posture from Cursor.
- Get remediation and secure-development guidance for engineering work.
- Start security design reviews and submit Markdown security reports.
- Confirm actions that submit content or start hosted work in Pi.
- Set up and manage the plugin through Cursor's **Customize** page.
