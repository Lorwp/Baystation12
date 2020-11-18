All users are expected to review [/docs/CODE_OF_CONDUCT.md](/docs/CODE_OF_CONDUCT.md) before interacting with the repository or other users.

Baystation12 is licensed under the GNU Affero General Public License version 3, which can be found in full in LICENSE-AGPL3.txt.

Commits with a git authorship date prior to `1420675200 +0000` (2015/01/08 00:00 GMT) are licensed under the GNU General Public License version 3, which can be found in full in LICENSE-GPL3.txt.

All commits whose authorship dates on or after `1420675200 +0000` are assumed to be licensed under AGPL v3, if you wish to license under GPL v3 please make this clear in the commit message and any added files.

## Running CI Locally

Requires [`act`](https://github.com/nektos/act) and Docker (with WSL2 enabled on Windows)

Needs to pull [`nektos/act-environments-ubuntu:18.04`](https://hub.docker.com/r/nektos/act-environments-ubuntu/tags), which at the time of writing is 18.2GB uncompressed (!!!).

```bash
# Run full CI suite
$ act
# Run only Dreamchecker
$ act -j DreamChecker
# Run only Code Tests
$ act -j Code
# Run only Map Tests
$ act -j Maps
```