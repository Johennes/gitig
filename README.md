# GitiG

GitiG is a shell script for mirroring an arbitrary git repository to GitHub and GitLab.

## Features

- Mirrors repositories to GitHub and GitLab
- Automatically creates / updates mirrored repositories as needed via the API
- Reads and replicates repository description from Gitea (if applicable)
- Works on existing checkout, no separate `--mirror` checkout needed
- Fully client-side, no access to the git server needed

## Why you should mirror

If you're self-hosting your repositories, mirroring them can help increase availability and reduce load on your own instance. It's also a way of backing up and increases redundancy.

The latter point might also be relevant to you if you're not self-hosting. There is nothing wrong with GitHub or GitLab. In fact, given the value they offer to users free of charge, these are great services. It's crucial to keep in mind though that precisely because you don't pay them, you don't truly control anything you push to their servers. The availability of whatever you enter on or upload to their site is at their own and only their own discretion.

A few noteworthy examples:

In October 2020 GitHub took down the popular youtube-dl repository alongside a number of forks in response to a [DMCA] notice.

In October 2019 GitLab tried to roll out an update to its terms of service that required opting into telemetry. If you didn't want to accept these new terms, you would have lost access to their website. (It's worth noting that, fortunately, they were sensitive to the community outrage following the announcement and [revised their plans] about a week later.)

## License

GitiG is licensed under the GNU General Public License as published
by the Free Software Foundation, either version 3 of the License, or (at your option) any
later version.

[revised their plans]: https://about.gitlab.com/blog/2019/10/10/update-free-software-and-telemetry/
[DMCA]: https://github.com/github/dmca/blob/master/2020/10/2020-10-23-RIAA.md