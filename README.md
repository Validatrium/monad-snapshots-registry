# Monad Snapshots Registry

This repository contains a list of public snapshots for monad-testnet provided by different validators.

## How to Add Your Snapshot

1. Create a **fork** of this repository.
2. Copy the file `validators/template.json`  into a new file `validators/<your-validator-name>.json`
3. Fill in the following fields::
   - `validator`
   - `network name` (mainnet or testnet)
   - `snapshot.block`
   - `snapshot.url`
   - `snapshot.checksum_url`
   - `snapshot.size`
   - `snapshot.compression`
   - `snapshot.updated_at` (UTC, ISO8601 format)

4. Commit your changes `git commit` and `push` them to your fork. 
5. Open a **Pull Request** to this repository.

## How to Update Your Snapshot

1. Update the fields in your file `validators/<your-validator-name>.json`:
   - `snapshot.block`
   - `snapshot.url`
   - `snapshot.checksum_url`
   - `snapshot.size`
   - `snapshot.updated_at`
2. Create a new Pull Request with the updated file.

Once the PR is merged, our Discord bot will automatically pull the updated data and announce the new snapshot
