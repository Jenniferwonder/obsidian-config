---

database-plugin: basic

---

```yaml:dbfolder
name: new database
description: new description
columns:
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
    position: 1
    isHidden: false
    sortIndex: -1
    width: 204
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
    isHidden: true
    position: 3
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
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 153
    options:
      - { label: "🟢Normal", value: "🟢Normal", color: "hsl(179,96%,90%)"}
      - { label: "🟡Risky", value: "🟡Risky", color: "hsl(51,96%,90%)"}
      - { label: "🟠Overdue", value: "🟠Overdue", color: "hsl(27,96%,90%)"}
      - { label: "🔵Done", value: "🔵Done", color: "hsl(109, 95%, 90%)"}
      - { label: "🤍ToPlan", value: "🤍ToPlan", color: "hsl(289, 95%, 90%)"}
      - { label: "💚ToDo", value: "💚ToDo", color: "hsl(301, 95%, 90%)"}
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
  Progress:
    input: rollup
    accessorKey: Progress
    key: Progress
    id: Progress
    label: Progress
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 152
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
      asociated_relation_id: Tasks
      rollup_action: Original Value
      rollup_key: status
  Score(0-1):
    input: rollup
    accessorKey: Score(0-1)
    key: Score(0-1)
    id: Score(0-1)
    label: Score(0-1)
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 122
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: true
      asociated_relation_id: Tasks
      rollup_action: Original Value
      wrap_content: false
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
    position: 7
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
  GoodParts:
    input: rollup
    accessorKey: GoodParts
    key: GoodParts
    id: Review(Good_Parts)
    label: Good Parts
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 165
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: true
      asociated_relation_id: Tasks
      rollup_action: Original Value
      rollup_key: GoodParts
  ToImprove:
    input: rollup
    accessorKey: ToImprove
    key: ToImprove
    id: Review(To_Improve)
    label: To Improve
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 173
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: true
      asociated_relation_id: Tasks
      rollup_action: Original Value
      rollup_key: ToImprove
  Completed:
    input: number
    accessorKey: Completed
    key: Completed
    id: Completed
    label: Completed
    position: 13
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
  Total:
    input: number
    accessorKey: Total
    key: Total
    id: Total
    label: Total
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
  Tasks:
    input: relation
    accessorKey: Tasks
    key: Tasks
    id: Tasks
    label: 对应Tasks
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 174
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: OKRTs/Tasks/DB-Tasks.md
      bidirectional_relation: false
      wrap_content: true
  Objective:
    input: relation
    accessorKey: Objective
    key: Objective
    id: Objective
    label: 对齐Objective
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 160
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: OKRTs/Objectives/DB-Objectives.md
      bidirectional_relation: true
      wrap_content: true
  Incomplete:
    input: number
    accessorKey: Incomplete
    key: Incomplete
    id: InComplete
    label: Incomplete
    position: 14
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
  Topic:
    input: rollup
    accessorKey: Topic
    key: Topic
    id: Topic
    label: Topic
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 114
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: true
      asociated_relation_id: Objective
      rollup_action: Original Value
      rollup_key: Topic
      wrap_content: true
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
  show_metadata_outlinks: true
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: OKRTs/KRs
  row_templates_folder: zz-templates/tp/tp-KRs
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
        label: "O1-Front-End"
        color: "hsl(200, 95%, 90%)"
        filters:
        - field: Objective
          operator: CONTAINS
          value: "O1"
          type: relation
      - condition: AND
        disabled: true
        label: "O2-PKM"
        color: "hsl(345, 95%, 90%)"
        filters:
        - field: Objective
          operator: CONTAINS
          value: "O2"
          type: relation
      - condition: AND
        disabled: true
        label: "O3-PMP"
        color: "hsl(233, 95%, 90%)"
        filters:
        - field: Objective
          operator: CONTAINS
          value: "O3"
          type: relation
```