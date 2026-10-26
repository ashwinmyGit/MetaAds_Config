# MetaAds_Config

Public hosting for the Meta Ads remote config and promo assets only. No source code, no production ad IDs.

- `remote-config.json` - the live config (Google test IDs / placeholders only)
- `fixtures/` - QA files for device tests (valid variants, partial, wrong-type, malformed)

Field reference: `Documentation~/RemoteConfigReference.md` in the Unity package.

## Categories

Exactly three, case-insensitive: `Puzzle`, `Action`, `Racing`. The same category selects the `Category` cross-promo list and
the `Notifications` list. A blank or unsupported category falls back to the project's local Category setting, then to none
(ads work; no promos or notifications). Apps with `_confirm_category` still need their category confirmed.
