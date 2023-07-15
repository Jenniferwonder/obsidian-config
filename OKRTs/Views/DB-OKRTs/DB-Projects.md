---
database-plugin: basic
---

```yaml:dbfolder
name: DB-Tasks
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
    position: 2
    isHidden: false
    sortIndex: -1
    width: 140
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
  DateStarted:
    input: calendar
    accessorKey: DateStarted
    key: DateStarted
    id: DateStarted
    label: DateStarted
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 117
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
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 135
    options:
      - { label: "💚ToDo", value: "💚ToDo", color: "hsl(127,100%,90%)"}
      - { label: "🟡ToOrganize", value: "🟡ToOrganize", color: "hsl(47,96%,90%)"}
      - { label: "🟠ToPublish", value: "🟠ToPublish", color: "hsl(6,96%,90%)"}
      - { label: "🟣Maintained", value: "🟣Maintained", color: "hsl(256,96%,90%)"}
      - { label: "🟢Published", value: "🟢Published", color: "hsl(99,96%,90%)"}
      - { label: "🔵Archived", value: "🔵Archived", color: "hsl(214,80%,88%)"}
      - { label: "⤵️Snooze", value: "⤵️Snooze", color: "hsl(165, 95%, 90%)"}
      - { label: "🤍ToPlan", value: "🤍ToPlan", color: "hsl(57,85%,95%)"}
      - { label: "💛ToCheck", value: "💛ToCheck", color: "hsl(38,96%,90%)"}
      - { label: "💙ToAct", value: "💙ToAct", color: "hsl(200,96%,90%)"}
      - { label: "⚪Backlog", value: "⚪Backlog", color: "hsl(99, 95%, 90%)"}
      - { label: "Sprint Backlog", value: "Sprint Backlog", color: "hsl(114, 95%, 90%)"}
      - { label: "🟡Organizing", value: "🟡Organizing", color: "hsl(282, 95%, 90%)"}
      - { label: "PKM Backlog", value: "PKM Backlog", color: "hsl(195, 95%, 90%)"}
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
  Owner:
    input: select
    accessorKey: Owner
    key: Owner
    id: Owner
    label: Owner
    position: 14
    skipPersist: false
    isHidden: true
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
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: 1
    width: 90
    isSorted: true
    isSortedDesc: false
    options:
      - { label: "P1", value: "P1", color: "hsl(19, 95%, 90%)"}
      - { label: "P0", value: "P0", color: "hsl(67, 95%, 90%)"}
      - { label: "P2", value: "P2", color: "hsl(42, 95%, 90%)"}
      - { label: "P3", value: "P3", color: "hsl(338, 95%, 90%)"}
      - { label: "P4", value: "P4", color: "hsl(2, 95%, 90%)"}
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
  title:
    input: text
    accessorKey: title
    key: title
    id: title
    label: Title
    position: 3
    skipPersist: false
    isHidden: true
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
  DateDue:
    input: calendar
    accessorKey: DateDue
    key: DateDue
    id: due
    label: DateDue
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 104
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
    position: 7
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 103
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  KRs:
    input: relation
    accessorKey: KRs
    key: KRs
    id: Tasks
    label: 对齐KRs
    position: 12
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 117
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
      bidirectional_relation: true
      wrap_content: true
  Objective:
    input: relation
    accessorKey: Objective
    key: Objective
    id: 对齐Objective
    label: 对齐Objective
    position: 13
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 107
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: OKRTs/Objectives/DB-Objectives.md
      bidirectional_relation: true
      wrap_content: true
  Completion:
    input: checkbox
    accessorKey: Completion
    key: Completion
    id: Completion
    label: Completion
    position: 10
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
    input: number
    accessorKey: Total
    key: Total
    id: Total
    label: Total
    position: 17
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
  Completed:
    input: number
    accessorKey: Completed
    key: Completed
    id: Completed
    label: Completed
    position: 18
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
    input: number
    accessorKey: Incomplete
    key: Incomplete
    id: Incomplete
    label: Incomplete
    position: 19
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: -278
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
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
    isHidden: true
    sortIndex: -1
    width: 199
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Progress:
    input: formula
    accessorKey: Progress
    key: Progress
    id: Progress
    label: Progress
    position: 24
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
      persist_changes: true
      formula_query: ${+row.Completed/+row.Total*100}%
  Estimated-Time:
    input: text
    accessorKey: Estimated-Time
    key: Estimated-Time
    id: Estimated-Time
    label: Estimated-Time
    position: 8
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
      persist_changes: false
  ToImprove:
    input: text
    accessorKey: ToImprove
    key: ToImprove
    id: ToImprove
    label: To Improve
    position: 20
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: false
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Topic:
    input: tags
    accessorKey: Topic
    key: Topic
    id: Topic
    label: Topic
    position: 1
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 155
    options:
      - { label: "Codespace", value: "Codespace", color: "hsl(32, 95%, 90%)"}
      - { label: "PKM-Productivity", value: "PKM-Productivity", color: "hsl(216, 95%, 90%)"}
      - { label: "PMP", value: "PMP", color: "hsl(13, 95%, 90%)"}
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
  ToKeep:
    input: text
    accessorKey: ToKeep
    key: ToKeep
    id: Check
    label: To Keep
    position: 16
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: false
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  Unexpected:
    input: text
    accessorKey: Unexpected
    key: Unexpected
    id: Unexpected
    label: Unexpected
    position: 21
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: false
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Score:
    input: number
    accessorKey: Score
    key: Score
    id: Score(0-1)
    label: Score(0-1)
    position: 15
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 96
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Outcomes:
    input: text
    accessorKey: Outcomes
    key: Outcomes
    id: Act
    label: Outcomes
    position: 22
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: false
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Resources:
    input: text
    accessorKey: Resources
    key: Resources
    id: Resource
    label: Resources
    position: 23
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
  show_metadata_DateModified: false
  show_metadata_tasks: true
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: tag
  source_form_result: "#Codespace,#PKM,#PMP,#Content-Making,#Design,#AI"
  source_destination_path: OKRTs/Tasks
  row_templates_folder: zz-templates/tp/tp-Task
  current_row_template: zz-templates/tp/tp-Tasks.md
  pagination_size: 200
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
      - condition: OR
        disabled: false
        label: "Active"
        color: "hsl(243, 95%, 90%)"
        filters:
        - field: status
          operator: CONTAINS
          value: "ToDo"
          type: select
        - field: status
          operator: CONTAINS
          value: "ToOrganize"
          type: select
        - field: status
          operator: CONTAINS
          value: "ToPublish"
          type: select
      - condition: AND
        disabled: true
        label: "Maintained"
        color: "hsl(27, 95%, 90%)"
        filters:
        - field: status
          operator: CONTAINS
          value: "Maintained"
          type: select
      - condition: OR
        disabled: true
        label: "Done"
        color: "hsl(204, 95%, 90%)"
        filters:
        - field: status
          operator: CONTAINS
          value: "Published"
          type: select
        - field: status
          operator: CONTAINS
          value: "Archived"
          type: select
      - condition: OR
        disabled: true
        label: "Snooze"
        color: "hsl(97, 95%, 90%)"
        filters:
        - field: status
          operator: CONTAINS
          value: "Snooze"
          type: select
        - field: status
          operator: IS_EMPTY
          value: ""
          type: select
      - condition: AND
        disabled: true
        label: "Codespace"
        color: "hsl(273, 95%, 90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "Codespace"
          type: text
      - condition: AND
        disabled: true
        label: "PKM"
        color: "hsl(302, 95%, 90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "PKM"
          type: text
      - condition: AND
        disabled: true
        label: "Content-Making"
        color: "hsl(9, 95%, 90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "Content-Making"
          type: text
      - condition: AND
        disabled: true
        label: "Design"
        color: "hsl(322, 95%, 90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "Design"
          type: text
      - condition: AND
        disabled: true
        label: "PMP"
        color: "hsl(150, 95%, 90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "PMP"
          type: text
      - condition: AND
        disabled: true
        label: "English-Improving"
        color: "hsl(236, 95%, 90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "English"
          type: text
```
