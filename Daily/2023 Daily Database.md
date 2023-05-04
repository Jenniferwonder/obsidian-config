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
    position: 5
    isHidden: false
    sortIndex: -1
    width: 191
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  title:
    input: text
    accessorKey: title
    key: title
    id: title
    label: Title
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 347
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Topic:
    input: text
    accessorKey: Topic
    key: Topic
    id: Topic
    label: Topic
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 187
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  周报:
    input: relation
    accessorKey: 周报
    key: 周报
    id: 周报
    label: 周报
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
      related_note_path: Tasks/Tasks Database.md
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