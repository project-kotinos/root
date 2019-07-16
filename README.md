## Instructions for migrating projects to YourBase
1. Download and install `yb` from https://dl.equinox.io/yourbase/yb/stable
2. Pick the next available 10 projects from the spreadsheet here: https://docs.google.com/spreadsheets/d/1XG7ufe_mQUYo7ZUmI0twirpBXjCvDi56HYT7ojjnoGE/edit?usp=sharing Put your name in the **yb contact** column for those projects.
3. Clone each project and convert the `.travis.yml` to Yourbase YAML. (Follow the documentation here: https://yourbase-docs-staging.s3-us-west-2.amazonaws.com/configuration/yourbase_yaml.html )
4. Run `yb build` for each project.
    1. If the conversion is successful, push the converted Yourbase YAML to GitHub and add a **Yes** in the **converted?** column.
    2. If the conversion is unsuccessful and if it’s due to a limitation in **yb**, create an issue in https://github.com/microclusters/issues/issues and put a link to the issue URL in the **remarks** column for that repo.
    3. If you had to tweak or skip some parts in the Travis YAML to work in YourBase, please note them down in the **remarks** column for that repo.
5. During this exercise if you found that YourBase docs can be improved, submit a PR to <YOURBASE_DOCS>
