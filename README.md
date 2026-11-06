# arena-coach-data

Pinned data inputs for arena-coach, served as Release assets. arena-coach's loader fetches each one by sha256 into a
local cache; the manifest in arena-coach (`data/phase-export.toml`) names the asset and its hash.

- `phase-export-<phase commit>`: a phase card-data export (https://github.com/phase-rs/phase), generated with phase's
  own `scripts/gen-card-data.sh` at that commit from MTGJSON data. phase is MIT OR Apache-2.0; MTGJSON data is MIT.

Assets are never replaced: a new input gets a new release, through arena-coach's upgrade procedure.
