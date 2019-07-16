## Instructions for migrating projects to YourBase
1. Download and install `yb` from https://dl.equinox.io/yourbase/yb/stable
2. Go to this link and pick an issue from the Milestone that's closest to completion. https://github.com/project-kotinos/issues/milestones?direction=desc&sort=completeness&state=open (i.e., Don't go to Batch 2 if Bactch 1 is incomplete.)
3. Assign the issue to yourself.
3. Clone the project that is mentioned in the issue description and convert the `.travis.yml` to Yourbase YAML. (Follow the documentation here: https://yourbase-docs-staging.s3-us-west-2.amazonaws.com/configuration/yourbase_yaml.html )
4. Run `yb build` for the project that you converted.
    1. If the conversion is successful, push the converted Yourbase YAML to GitHub and mark the respective issue as fixed.
    2. If the conversion is unsuccessful and if it’s due to a limitation in **yb**, create an issue in https://github.com/microclusters/issues/issues and link to in the current issue as a comment.
    3. If you had to tweak or skip some parts in the Travis YAML for it to work in YourBase, mention that as a comment in the current issue.
5. During this exercise if you found that YourBase docs can be improved, submit a PR to https://github.com/yourbase/ybdocs.
6. Repeat until all milestones are completed.
