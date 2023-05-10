---
database-plugin: basic
---

```yaml:dbfolder
name: 2023-Daily-Database
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
    sortIndex: 1
    width: 103
    isSorted: true
    isSortedDesc: true
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: false
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
    width: 171
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  Topic:
    input: tags
    accessorKey: Topic
    key: Topic
    id: Topic
    label: Topic
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 198
    options:
      - { label: "Codespace", value: "Codespace", color: "hsl(311, 95%, 90%)"}
      - { label: "Life-Tricks", value: "Life-Tricks", color: "hsl(104,96%,90%)"}
      - { label: "Content-Making", value: "Content-Making", color: "hsl(179,96%,90%)"}
      - { label: "English-Improving", value: "English-Improving", color: "hsl(67,96%,90%)"}
      - { label: "PKM-Productivity", value: "PKM-Productivity", color: "hsl(38,96%,90%)"}
      - { label: "OKRTs", value: "OKRTs", color: "hsl(4, 95%, 90%)"}
      - { label: "AI", value: "AI", color: "hsl(346, 95%, 90%)"}
      - { label: "PMP", value: "PMP", color: "hsl(29, 95%, 90%)"}
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
      wrap_content: true
  Tasks:
    input: relation
    accessorKey: Tasks
    key: Tasks
    id: Tasks
    label: Tasks
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 162
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
      related_note_path: OKRTs/Tasks/Tasks Database.md
      bidirectional_relation: true
  __outlinks__:
    key: __outlinks__
    id: __outlinks__
    input: outlinks
    label: Outlinks
    accessorKey: __outlinks__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: false
    position: 6
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
  DateStarted:
    input: calendar
    accessorKey: DateStarted
    key: DateStarted
    id: DateStarted
    label: DateStarted
    position: 100
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
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: true
  show_metadata_tags: false
  source_data: tag
  source_form_result: "#Daily"
  source_destination_path: Daily
  row_templates_folder: zz-templates
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
filters:
  enabled: true
  conditions:
      - condition: AND
        disabled: true
        label: "1月"
        color: "hsl(213, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-01"
          type: text
      - condition: AND
        disabled: true
        label: "2月"
        color: "hsl(88, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-02"
          type: text
      - condition: AND
        disabled: true
        label: "3月"
        color: "hsl(230, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-03"
          type: text
      - condition: AND
        disabled: true
        label: "4月"
        color: "hsl(77, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-04"
          type: text
      - condition: AND
        disabled: false
        label: "5月"
        color: "hsl(65, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-05"
          type: text
```
