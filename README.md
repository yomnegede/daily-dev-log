# Daily Repository Snapshot

This repository records one transparent, automated snapshot of its GitHub
metadata each day. It is intentionally labeled as automation; it does not claim
that the generated entries are hand-written development work.

The snapshot includes the repository's stars, forks, open issues, and the commit
that was current when the workflow started. Entries are stored by month under
[`activity/`](activity/).

## Schedule

The workflow runs daily at 9:17 AM in `America/New_York`. The non-round minute
reduces the chance of GitHub Actions congestion. It can also be run manually
from the **Actions** tab.

## Contribution attribution

On every run, the workflow retrieves the numeric GitHub account ID for the
workflow actor and uses GitHub's private `noreply` address format for the commit.
The generated commit is pushed to the default branch using the repository's
built-in `GITHUB_TOKEN`; no personal access token is stored.

GitHub ultimately decides which activity qualifies for the profile contribution
graph. A qualifying commit normally needs to be on the default branch of a
standalone repository and use an email address associated with the account.

