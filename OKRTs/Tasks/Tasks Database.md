---

database-plugin: basic

---

```yaml:dbfolder
name: new database
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
    position: 2
    isHidden: false
    sortIndex: -1
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
    position: 3
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
  started:
    input: calendar
    accessorKey: started
    key: started
    id: started
    label: Started
    position: 6
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
  due:
    input: calendar
    accessorKey: due
    key: due
    id: due
    label: Due
    position: 7
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
  status:
    input: select
    accessorKey: status
    key: status
    id: status
    label: Status
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "🟡Organizing", value: "🟡Organizing", color: "hsl(149, 95%, 90%)"}
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
  对齐KR:
    input: relation
    accessorKey: 对齐KR
    key: 对齐KR
    id: 对齐KR
    label: 对齐KR
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: KRs/KR Database.md
      bidirectional_relation: true
  Owner:
    input: select
    accessorKey: Owner
    key: Owner
    id: Owner
    label: Owner
    position: 12
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Jennifer", value: "Jennifer", color: "hsl(249, 95%, 90%)"}
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
  Priority:
    input: select
    accessorKey: Priority
    key: Priority
    id: Priority
    label: Priority
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
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
  Tasks:
    input: relation
    accessorKey: Tasks
    key: Tasks
    id: Tasks
    label: 日报
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 133
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
      related_note_path: Daily/2023 Daily Database.md
      bidirectional_relation: true
  title:
    input: text
    accessorKey: title
    key: title
    id: title
    label: Title
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 201
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  对齐Objective:
    input: relation
    accessorKey: 对齐Objective
    key: 对齐Objective
    id: 对齐Objective
    label: 对齐Objective
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 134
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: OKRTs/Objectives/Objectives Database.md
      bidirectional_relation: true
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: true
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: tag
  source_form_result: "#Tasks"
  source_destination_path: OKRTs/Tasks
  row_templates_folder: zz-templates
  current_row_template: zz-templates/tp/tp-Tasks.md
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
filters:
  enabled: false
  conditions:
```