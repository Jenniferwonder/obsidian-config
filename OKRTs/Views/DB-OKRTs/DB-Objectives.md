---
database-plugin: basic
---

```yaml:dbfolder
name: DB-Objective
description: new description
columns:
  column1:
    input: text
    key: column1
    accessorKey: column1
    label: Column 1
    position: 1
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 3
    isHidden: false
    sortIndex: -1
    width: 188
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  __tasks__:
    key: __tasks__
    id: __tasks__
    input: task
    label: Task
    accessorKey: __tasks__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: false
    position: 4
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  status:
    input: select
    accessorKey: status
    key: status
    id: status
    label: Status
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: 1
    width: 141
    isSorted: true
    isSortedDesc: true
    options:
      - { label: "🟢Normal", value: "🟢Normal", color: "hsl(87,96%,90%)"}
      - { label: "🟡Risky", value: "🟡Risky", color: "hsl(47,96%,90%)"}
      - { label: "🟠Overdue", value: "🟠Overdue", color: "hsl(0,96%,90%)"}
      - { label: "🤍ToPlan", value: "🤍ToPlan", color: "hsl(251, 95%, 90%)"}
      - { label: "💚ToDo", value: "💚ToDo", color: "hsl(133, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
  DateStarted:
    input: calendar
    accessorKey: DateStarted
    key: DateStarted
    id: DateStarted
    label: DateStarted
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  DateDue:
    input: calendar
    accessorKey: DateDue
    key: DateDue
    id: due
    label: DateDue
    position: 12
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  DateDo:
    input: calendar
    accessorKey: DateDo
    key: DateDo
    id: DateDo
    label: DateDo
    position: 13
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Tasks:
    input: relation
    accessorKey: Tasks
    key: Tasks
    id: 对齐Objective
    label: Tasks
    position: 6
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 216
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: OKRTs/Tasks/Tasks Database.md
      bidirectional_relation: true
      wrap_content: true
  Completed:
    input: text
    accessorKey: Completed
    key: Completed
    id: Completed
    label: Completed
    position: 15
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Total:
    input: text
    accessorKey: Total
    key: Total
    id: Total
    label: Total
    position: 14
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Incomplete:
    input: text
    accessorKey: Incomplete
    key: Incomplete
    id: InComplete
    label: Incomplete
    position: 16
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Rollup:
    input: rollup
    accessorKey: Rollup
    key: Rollup
    id: Rollup
    label: Rollup
    position: 7
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: true
      asociated_relation_id: 
      rollup_action: Original Value
      rollup_key: Progress
  KR1:
    input: relation
    accessorKey: KR1
    key: KR1
    id: Objective
    label: KR1
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 249
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: OKRTs/KRs/DB-KRs.md
      bidirectional_relation: false
      wrap_content: true
  KR2:
    input: relation
    accessorKey: KR2
    key: KR2
    id: KR2
    label: KR2
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 185
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: OKRTs/KRs/DB-KRs.md
      bidirectional_relation: false
      wrap_content: true
  Topic:
    input: select
    accessorKey: Topic
    key: Topic
    id: Topic
    label: Topic
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 152
    options:
      - { label: "PKM-Productivity", value: "PKM-Productivity", color: "hsl(113,96%,90%)"}
      - { label: "Codespace", value: "Codespace", color: "hsl(176,96%,90%)"}
      - { label: "PMP", value: "PMP", color: "hsl(245, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_DateModified: false
  show_metadata_tasks: true
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: OKRTs/Objectives
  row_templates_folder: zz-templates/tp/tp-Objective
  current_row_template: 
  pagination_size: 40
  font_size: 16
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: false
  implementation: default
  show_metadata_modified: false
filters:
  enabled: true
  conditions:
```
