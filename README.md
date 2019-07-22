## Instructions for migrating projects to YourBase
1. Download and install `yb` from https://dl.equinox.io/yourbase/yb/stable
2. Go to [this](https://github.com/project-kotinos/issues/milestones?direction=desc&sort=completeness&state=open) link and pick an issue from the Milestone that's closest to completion.  (i.e., Don't go to Batch 2 if Batch 1 is incomplete.)
3. Assign the issue to yourself.
4. Clone the project that is mentioned in the issue description.
5. Convert the `.travis.yml` to Yourbase YAML. (Follow the documentation here: https://yourbase-docs-staging.s3-us-west-2.amazonaws.com/configuration/yourbase_yaml.html ) Always use the`.travis.yml` from the most recent passing build of `master` branch for migration. If there is no `master` branch, pick the branch with the most recent passing build.
6. Run `yb build` for the project that you just converted.
    1. If the conversion is successful, push the converted Yourbase YAML to GitHub and mark the respective issue as fixed.
    2. If the conversion is unsuccessful and if it’s due to a limitation in **yb**, create an issue in https://github.com/microclusters/issues/issues and link to it in the current issue as a comment.
    3. If you had to tweak or skip some parts in the Travis YAML for it to work in YourBase, mention that as a comment in the current issue.
7. During this exercise if you found that YourBase docs can be improved, submit a PR to https://github.com/yourbase/ybdocs.
8. Repeat until all milestones are completed.
