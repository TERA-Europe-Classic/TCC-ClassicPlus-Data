# TCC Classic+ Data

Generated runtime databases for TERA Europe Classic+ TCC.

Source datacenter folders expected under the Classic+ client repository:

- `Client\DataCenter_Final_EUR`
- `Client\DataCenter_Final_FRA`
- `Client\DataCenter_Final_GER`
- `Client\DataCenter_Final_RUS`

Regenerate from the TCC repository:

```powershell
python tools\generate_tcc_classicplus_data.py --elinu-root <classic-plus-repo-root> --out-dir <output-data-dir> --hashes <database-hashes.json>
```

The raw file layout is intentionally flat at the repository root because TCC downloads files by relative database path.
