# agent-og-auto-merge-test

Test repository for exercising the [auto-merge-agent](https://github.com/opendatahub-io/auto-merge-agent)
GitHub App deployment.

Pull requests that only touch `README.md` or files under `docs/` and pass the
`tests` CI check are eligible for automatic squash merge.

## Test plan

1. The auto-merge-agent evaluates this pull request against the
   `docs-only` rule in its policy.
2. With the `tests` CI check green and a completed CodeRabbit review,
   the agent squash-merges the change without human review.
