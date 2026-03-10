# meeting-focus-releases

Public release feed for MeetingAttentionFilter.

## Layout

- `latest.json`: manifest consumed by update tooling.
- `releases-index.json`: historical release manifest entries.
- `releases/<version>/release-info.json`: version metadata.
- `releases/<version>/release-notes.md`: markdown notes.
- `releases/<version>/MeetingAttentionFilter-Setup.exe`: installer asset.

## Automated release from tag

Workflow: `.github/workflows/release-from-tag.yml`

Trigger:

- Push tag in format `v<version>` such as `v1.0.0`, `v1.0.0a`, `v1.0.0b`.

Required files in tagged commit:

- `releases/<version>/MeetingAttentionFilter-Setup.exe`
- `releases/<version>/release-info.json`
- `releases/<version>/release-notes.md`
