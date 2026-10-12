# Source release manifest

## Purpose and origin

Unpublished, history-free, source-only DecisionAI AI Engineering portfolio candidate. Originating complete source SHA: `09f15b549c60b8703123624e5a9ff92fd9e4ac39`.

## Fixed export scope

The initial export contained exactly **252 regular files**: all 253 regular-file blobs in the fixed source tree except `.github/workflows/deploy.yml`. No original `.git` history or metadata was copied. Ignored/untracked provider artifacts, credentials, environments, caches, logs and raw data were not exported. The included CI workflow has no AWS deployment stage.

Export groups: 101 application files, 100 test files, 28 documentation files, 7 scripts, 3 synthetic CSV files, 1 CI workflow and 12 root files. This manifest is an additional candidate-only file, making the expected candidate total 253.

## Candidate-only changes

- `README.md`: source-only identity, provenance and omitted deployment workflow.
- `AGENTS.md`: historical deployment guidance rather than an included executable workflow.
- `docs/coding-agent-lab.md`: originating-repository exercise attribution.
- `docs/docker-cicd-cloud.md`: historical operational scope.
- `docs/portfolio-release-evidence.md`: snapshot provenance, corrected workflow references, completed reconciliation/MIT decisions and separate later test results.
- `.github/workflows/ci.yml`: approved workflow-level token hardening to `permissions: contents: read`.
- `docs/source-release-manifest.md`: this new record.

Application code, tests, scripts, datasets, dependency locks, LICENSE and Dockerfiles remain source-identical. CI differs only by the explicit read-only token policy; its triggers, jobs, steps and execution order are unchanged. The MIT LICENSE and approved copyright attribution are retained unchanged. ADR-006 remains Proposed.

## Deterministic inventory and hashes

Derive the original inventory from `git ls-tree -r` of the complete originating SHA, exclude the deployment workflow, and sort relative paths ordinally. For each entry, read raw bytes using its Git blob ID; compute SHA-256 for source bytes and candidate bytes. Record relative path, source blob ID, source SHA-256, candidate SHA-256 and whether it is an approved documentation or CI-permission adaptation. For the new manifest, use no source hash. Do not hash decoded text or normalize line endings.

The controlled export verified all 252 original files against their raw Git blob identities. That is not a published SHA-256 inventory. No per-file SHA-256 values are fabricated here; a serialized hash inventory remains to be recorded under separate approval. Subsequent integrity review must require byte identity for all unchanged files and list only the approved documentation and CI-permission differences.

## Historical evidence

See [portfolio evidence](portfolio-release-evidence.md) for originating Phase 19.2 checks: 741 tests, recorded Decimal calculations and dataset SHA-256 identities. The later qualitative-review discovery correction separately recorded 748 tests. Human-executed reproduction and historical provider/delivery summaries retain their own provenance. None is a fresh execution in this candidate. Original commit history and local provider artifacts are unavailable here; originating SHAs are provenance identifiers, not links to included commits.

## New candidate validation status

- Controlled export: 252 files; raw Git blob identity verified; deployment omitted and CI retained.
- Candidate documentation/integrity/link review: performed during adaptation; results reported separately for human review.
- Candidate Python 3.14.6 and candidate application import origin: **verified**. Existing installed versions match 67 production and 73 development entries; no fresh installation was performed.
- Qualitative-review collection and tests: **7 collected and 7 passed**, exit 0.
- Evaluation tests: **123 passed, 1 warning**, exit 0; Ruff: **passed**, exit 0; full pytest: **748 passed, 1 warning in 31.80s**, exit 0. Plugins, bytecode and repository caches were disabled.
- Candidate standard-library Decimal reproduction: **passed**, exit 0; all row counts and numerical results match historical evidence. Candidate LF CSV hashes differ from historical CRLF working-copy hashes; normalized text is identical and candidate bytes match the originating Git blobs. See [candidate results](portfolio-release-evidence.md#independent-public-candidate-verification--phase-194) for exact commands, hashes, figures and limitations.
- Clean-environment installation and lock freshness: **not run**.
- Docker builds: **not run**.
- Candidate CI execution: **not run**.
- Independent Mermaid rendering/parser validation: **unverified**.
- Provider quality, AWS runtime and production readiness: **unverified**.

After both execution steps, all 253 candidate hashes were unchanged, no unexpected candidate files appeared, and the operational repository remained clean. At that execution baseline, code, tests, CSVs, scripts, locks, LICENSE, Dockerfiles and CI retained source identity; subsequent CI hardening is recorded separately below. Git history and deployment remain absent. This later evidence update modifies only the manifest and portfolio evidence document; no additional checks were executed.

## Current source-identity accounting and CI hardening

The current candidate contains **253 files**: **246 files match originating Git blobs exactly**, **six exported files have approved candidate-only modifications**, and **one manifest is candidate-only**. The six modified originals are `README.md`, `AGENTS.md`, `docs/portfolio-release-evidence.md`, `docs/coding-agent-lab.md`, `docs/docker-cicd-cloud.md`, and `.github/workflows/ci.yml`. Application source, tests, scripts, synthetic CSVs, dependency locks, LICENSE and Dockerfiles remain byte-identical to the fixed originating source. The CI workflow is no longer byte-identical.

The approved workflow-level policy is:

```yaml
permissions:
  contents: read
```

YAML structure was manually inspected. Removing this block reproduces the previous workflow exactly; all triggers, jobs, actions, installation commands, lock checks, tests and Docker build steps are preserved. Automated YAML parsing has **not been executed**, and the candidate GitHub Actions workflow has **not been executed**. No AWS deployment action or workflow is included. Prior candidate pytest, Ruff and Decimal results remain unchanged and precede this permissions-only edit; they are not a fresh workflow execution or build verification.

## Remaining release limitations

Exact locked-dependency attribution review, final privacy/public-disclosure approval, outstanding installation/lock/build/CI checks and explicit publication approval remain pending. Completed local test/lint/arithmetic validation is bounded to the existing verified environment. Source-only scope does not distribute installed dependencies or built images; any later binary/container distribution needs its own review. No recording, analyst validation, causal proof or broad reliability result is claimed. No Git repository has been initialized and this snapshot is not published.
