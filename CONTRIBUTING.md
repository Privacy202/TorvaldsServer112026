# Contributing

This repository holds several programs, one branch each. GitHub is a read-only copy, so pull
requests there are closed automatically. Changes are sent as patches by email to **patches@mytangle.ca**.

## Before you send

- **Sign off every commit.** Add a `Signed-off-by: Your Real Name <you@example.com>` line
  (`git commit -s` does it). It certifies the
  [Developer Certificate of Origin 1.1](https://developercertificate.org/): that you wrote the
  change or have the right to submit it. Patches without it are refused.
- **One logical change per patch.** Every patch in a series must build and work on its own.
- **Don't break what already works.** A change that breaks existing behaviour for users is a bug,
  whatever else it fixes.

## Sending patches

- Plain-text email, with the patch inline in the body rather than attached.
  `git send-email --to=patches@mytangle.ca` does this for you.
- Name the program's branch in the subject: `git format-patch --subject-prefix="PATCH <branch>"`.
- For more than one patch, include a cover letter as patch 0 (`--cover-letter`) explaining the series.
- For a revised series, label it v2, v3 and so on (`-v2`), and put what changed since the last
  version below the `---` line, so it stays out of the commit.

## Review

Reply inline, below the lines you're answering, not above the quoted message. Review tags are
recorded in the commit: `Reviewed-by`, `Acked-by`, `Tested-by`, `Reported-by`, `Fixes`
and `Link`.

See MAINTAINERS for who looks after what.
