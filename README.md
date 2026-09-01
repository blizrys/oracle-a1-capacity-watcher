# Oracle A1 Capacity Watcher

Retries launching an OCI Always Free Ampere A1 (VM.Standard.A1.Flex, 2 OCPU / 12 GB) instance
every 15 minutes via GitHub Actions until Oracle has capacity available.

Stops automatically once `SUCCESS` exists in the repo. Check `instance.json` and `public_ip.txt`
for the result. Run manually anytime from the Actions tab ("Run workflow").

Credentials are stored as encrypted repository secrets (Settings > Secrets and variables > Actions),
never committed to the repo.
