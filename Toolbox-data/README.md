# Toolbox Data

This repository hosts the external configuration data files used by the
DeadZone Toolbox app (`com.deadzone.toolbox`).

The app downloads these files at runtime from:

```
https://raw.githubusercontent.com/mohammedmezo99/DeadZoneToolbox-Data/main/Toolbox-data/<file>
```

## Files

| File | Purpose |
|------|---------|
| `Blacklist.txt` | Apps excluded from per-app spoofing / hidden features |
| `Keybox.xml` | Default keybox payload (kept identical to upstream) |
| `Pif-props.json` | Default Play Integrity Fix props (JSON) |
| `app-props.json` | Per-app spoofing profiles |
| `date-update.txt` | Last updated date string |
| `device-model.json` | Device-model catalog used by the spoofing screen |
| `edit_file.json` | Editable raw payload store |
| `quotes.txt` | Motivational quotes shown in the about screen |

## Notes

- `Keybox.xml` is preserved unchanged from the original baseline
  (MD5 `290023a1b7c63a97dca00ad46675d33b`).
- `Pif-props.json` carries the AlwaysStrong `pif_fallback_1.prop`
  fingerprint (Pixel 8 Pro / `husky_beta`) so the app has a sane
  default when no user profile is loaded.
- The folder layout matches upstream
  [Kaorios-Toolbox](https://github.com/Wuang26/Kaorios-Toolbox)
  `Toolbox-data/` organization.
