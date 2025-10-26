# Remove Groups (with confirmation)

- Each group header now has a subtle **trash icon button** (transparent, not red) to remove the group.
- Clicking it asks: **“Are you sure you want to remove the group … ? This will also delete its tasks.”**
- If confirmed, the group and its tasks are removed from storage and the UI updates.

Everything else remains:
- Add Group, Themes, collapsible sections (headers are drop targets), auto-scroll drag, precise insert positions, iOS safe-area & icon/manifest.

Implementation notes:
- Buttons use `.btn-group-delete` styles with the same SVG as task delete but muted color and transparent background.
- Data keys: `task-tracker:v13` (tasks), `task-tracker:groups` (order + titles), `task-tracker:collapsed` (per-group collapsed), `task-tracker:theme` (selected theme).
