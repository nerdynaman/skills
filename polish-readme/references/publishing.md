# Publishing

Read only for requested repository descriptions, commits/pushes or visibility changes. Follow the host environment’s tools and authorization rules; preserve the repository’s current visibility unless the user requests a change.

## Repository description

Write one concise sentence describing the actual purpose and its distinguishing platform or workflow. Match the README’s terminology. Update the remote description only when that metadata change is in scope, and verify the saved value.

## Commit and push

1. Inspect the branch, origin, working tree and staged changes. Preserve unrelated work and use the requested repository and branch.
2. Review the documentation/asset diff, including moved guides and catalogue updates. Stage the intended files explicitly.
3. Check the author identity before committing. Prefer the owner’s configured identity; if it is missing, a verified account’s no-reply identity can be scoped to this repository rather than exposing an inferred machine-local address.
4. Commit with a message describing the documentation change and push through the environment’s supported workflow. Handle a protected branch through its required review process. Keep force-pushes outside routine documentation updates.
5. Verify the pushed commit matches the remote target and report any remaining working-tree changes accurately.

## Visibility changes

Making a repository public exposes its history and release assets as well as the latest files. Before a requested private-to-public change, inspect those surfaces for credentials, private configuration and stored runtime data; include bundled archives when present. Report findings by path/type without reproducing secret values. A clean pattern scan is supporting evidence, not proof that every kind of sensitive information is absent.

Compare what will become public with the user’s requested scope. If unexpected sensitive content blocks publication, explain the concrete finding and the change needed. Preserve data and history until cleanup or rewriting is authorized.

Prepare and validate the documentation before changing visibility. Once publication is authorized and the content check is clear, apply the requested visibility and verify it directly. Keep deployments, running services, schedules and network access settings unchanged unless separately requested.
