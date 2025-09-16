# ScriptHookVDotNet-nightly
Mirror for CI builds.

Nightly gets an update for a release every commit pushed on [the main repository](https://github.com/scripthookvdotnet/scripthookvdotnet/commits/main).
Commit SHAs on tags are not important for artifacts on this nightly repository, as they only
reference commits on this nightly repository, which is rarely updated by commits.

The link in a release description refers to a commit in the main repository.

Starting from [v3.7.0-nightly.48](https://github.com/scripthookvdotnet/scripthookvdotnet-nightly/releases/tag/v3.7.0-nightly.48), binary archives/artifacts will not be modified once releases are published. Although immutable releases can be deleted, tags that are already used by ones cannot be recreated. Therefore, you can always obtain the same archive with the same version tag unless the release associated with the tag is deleted.
You can verify the integrity of them with their SHA-256 hashes or the GitHub CLI.
You can see how to verify with the GitHub CLI at [a article on GitHub Docs](https://docs.github.com/en/code-security/supply-chain-security/understanding-your-software-supply-chain/verifying-the-integrity-of-a-release). 

When you report bugs in the main repository, report with a commit in the main repository,
not a commit in this repository. The description in each release contains the short and full
hashes of the corresponding commit in the main repository. Reporting bugs with the short commit
hash is acceptable unless the main branch in the main repository contains multiple hashes starting
with the short commit hash (you could report with the full hash in this case).

For the commit history on the main repository, see https://github.com/scripthookvdotnet/scripthookvdotnet/commits/main.
