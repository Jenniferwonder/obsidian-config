---
database-plugin: basic
---

```yaml:dbfolder
name: DB-Daily 2022
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
    width: 84
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
  Topic:
    input: tags
    accessorKey: Topic
    key: Topic
    id: Topic
    label: Topic
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 146
    options:
      - { label: "Codespace", value: "Codespace", color: "hsl(311, 95%, 90%)"}
      - { label: "Life-Tricks", value: "Life-Tricks", color: "hsl(104,96%,90%)"}
      - { label: "Content-Making", value: "Content-Making", color: "hsl(179,96%,90%)"}
      - { label: "English-Improving", value: "English-Improving", color: "hsl(67,96%,90%)"}
      - { label: "PKM-Productivity", value: "PKM-Productivity", color: "hsl(38,96%,90%)"}
      - { label: "OKRTs", value: "OKRTs", color: "hsl(4, 95%, 90%)"}
      - { label: "AI", value: "AI", color: "hsl(346, 95%, 90%)"}
      - { label: "PMP", value: "PMP", color: "hsl(29, 95%, 90%)"}
      - { label: "TechSkills", value: "TechSkills", color: "hsl(5, 95%, 90%)"}
      - { label: "[[400-Areas/PKM/PKM.md|PKM]]", value: "[[400-Areas/PKM/PKM.md|PKM]]", color: "hsl(6, 95%, 90%)"}
      - { label: "[[300-Areas/PKM/PKM.md|PKM]]", value: "[[300-Areas/PKM/PKM.md|PKM]]", color: "hsl(231, 95%, 90%)"}
      - { label: "[[300-Areas/Content-Making/Content-Making.md|Content-Making]]", value: "[[300-Areas/Content-Making/Content-Making.md|Content-Making]]", color: "hsl(43, 95%, 90%)"}
      - { label: "[[400-Life/Travelling.md|Travelling]]", value: "[[400-Life/Travelling.md|Travelling]]", color: "hsl(248, 95%, 90%)"}
      - { label: "2023-05-28 Free Writing", value: "2023-05-28 Free Writing", color: "hsl(31, 95%, 90%)"}
      - { label: "[[300-Areas/00-Learning Strategy & Workflow/00-Learning Strategy & Workflow.md|00-Learning Strategy & Workflow]]", value: "[[300-Areas/00-Learning Strategy & Workflow/00-Learning Strategy & Workflow.md|00-Learning Strategy & Workflow]]", color: "hsl(19, 95%, 90%)"}
      - { label: "[[CCC-CPE/Free Writing/Free Writing.md|Free Writing]]", value: "[[CCC-CPE/Free Writing/Free Writing.md|Free Writing]]", color: "hsl(299, 95%, 90%)"}
      - { label: "[[100-TechSkills/100-TechSkills.md|100-TechSkills]]", value: "[[100-TechSkills/100-TechSkills.md|100-TechSkills]]", color: "hsl(332, 95%, 90%)"}
      - { label: "[[300-Areas/PM/PMP/PMP.md|PMP]]", value: "[[300-Areas/PM/PMP/PMP.md|PMP]]", color: "hsl(208, 95%, 90%)"}
      - { label: "[[400-Life/Traveling/Traveling.md|Traveling]]", value: "[[400-Life/Traveling/Traveling.md|Traveling]]", color: "hsl(290, 95%, 90%)"}
      - { label: "[[300-Areas/PKM/00-Learning Strategy & Workflow/00-Learning Strategy & Workflow.md|00-Learning Strategy & Workflow]]", value: "[[300-Areas/PKM/00-Learning Strategy & Workflow/00-Learning Strategy & Workflow.md|00-Learning Strategy & Workflow]]", color: "hsl(341, 95%, 90%)"}
      - { label: "[[400-Life/Health/Health& Fitness.md|Health& Fitness]]", value: "[[400-Life/Health/Health& Fitness.md|Health& Fitness]]", color: "hsl(258, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
      wrap_content: true
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
    position: 8
    isHidden: true
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
    position: 9
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
  ToKeep:
    input: text
    accessorKey: ToKeep
    key: ToKeep
    id: ToKeep
    label: ToKeep
    position: 10
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 115
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
  ToImprove:
    input: text
    accessorKey: ToImprove
    key: ToImprove
    id: ToImprove
    label: ToImprove
    position: 11
    skipPersist: false
    isHidden: true
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
  KRs:
    input: relation
    accessorKey: KRs
    key: KRs
    id: KRs
    label: KRs
    position: 5
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 96
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
  Objective:
    input: relation
    accessorKey: Objective
    key: Objective
    id: Objective
    label: Objective
    position: 4
    skipPersist: false
    isHidden: true
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
      related_note_path: OKRTs/Objectives/DB-Objectives.md
  Unexpected:
    input: text
    accessorKey: Unexpected
    key: Unexpected
    id: Unexpected
    label: Unexpected
    position: 12
    skipPersist: false
    isHidden: true
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
  Act:
    input: text
    accessorKey: Act
    key: Act
    id: Act
    label: Act
    position: 13
    skipPersist: false
    isHidden: true
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
    position: 7
    width: 225
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
  Title:
    input: text
    accessorKey: Title
    key: Title
    id: title
    label: Title
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 176
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
  Project:
    input: relation
    accessorKey: Project
    key: Project
    id: Tasks
    label: Tasks
    position: 14
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 114
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
      related_note_path: OKRTs/Tasks/DB-Tasks.md
      bidirectional_relation: true
  Read:
    input: text
    accessorKey: Read
    key: Read
    id: Read
    label: Read
    position: 23
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 118
    config:
      enable_media_view: true
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  Watched:
    input: text
    accessorKey: Watched
    key: Watched
    id: Watched
    label: Watched
    position: 24
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
  Review:
    input: text
    accessorKey: Review
    key: Review
    id: Review
    label: Review
    position: 26
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
      wrap_content: true
  Gains:
    input: text
    accessorKey: Gains
    key: Gains
    id: Gains
    label: Gains
    position: 32
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  People:
    input: text
    accessorKey: People
    key: People
    id: People
    label: People
    position: 29
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
  Places:
    input: text
    accessorKey: Places
    key: Places
    id: Places
    label: Places
    position: 30
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
  Code:
    input: text
    accessorKey: Code
    key: Code
    id: Code
    label: Code
    position: 25
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  Ideas:
    input: text
    accessorKey: Ideas
    key: Ideas
    id: Ideas
    label: Ideas
    position: 27
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  Publish:
    input: text
    accessorKey: Publish
    key: Publish
    id: Publish
    label: Publish
    position: 34
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 118
    config:
      enable_media_view: true
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  Improved:
    input: text
    accessorKey: Improved
    key: Improved
    id: Improved
    label: Improved
    position: 33
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  Working_on:
    input: text
    accessorKey: Working_on
    key: Working_on
    id: Working_on
    label: Working on
    position: 15
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 105
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
  Love:
    input: checkbox
    accessorKey: Love
    key: Love
    id: Love
    label: Love
    position: 16
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
  Learned:
    input: text
    accessorKey: Learned
    key: Learned
    id: Learned
    label: Learned
    position: 28
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
  Write:
    input: text
    accessorKey: Write
    key: Write
    id: Writing
    label: Write
    position: 31
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
  MorningExercise:
    input: checkbox
    accessorKey: MorningExercise
    key: MorningExercise
    id: MorningExercise
    label: MorningExercise
    position: 17
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: -35
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  EveningExercise:
    input: checkbox
    accessorKey: EveningExercise
    key: EveningExercise
    id: EveningExercise
    label: EveningExercise
    position: 18
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
  Aerobics:
    input: checkbox
    accessorKey: Aerobics
    key: Aerobics
    id: Aerobics
    label: Aerobics
    position: 19
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
  Strength:
    input: checkbox
    accessorKey: Strength
    key: Strength
    id: Strength
    label: Strength
    position: 20
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
  Shape:
    input: checkbox
    accessorKey: Shape
    key: Shape
    id: Shape
    label: Shape
    position: 21
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
  LunchAtHome:
    input: number
    accessorKey: LunchAtHome
    key: LunchAtHome
    id: LunchAtHome
    label: LunchAtHome
    position: 22
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
  show_metadata_tasks: true
  show_metadata_inlinks: false
  show_metadata_outlinks: true
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: 000-OKRTs/Daily
  row_templates_folder: 000-Templates
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
        label: "6月"
        color: "hsl(213, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2022-06"
          type: text
      - condition: AND
        disabled: true
        label: "7月"
        color: "hsl(88, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2022-07"
          type: text
      - condition: AND
        disabled: true
        label: "8月"
        color: "hsl(230, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2022-08"
          type: text
      - condition: AND
        disabled: true
        label: "9月"
        color: "hsl(77, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2022-09"
          type: text
      - condition: AND
        disabled: true
        label: "10月"
        color: "hsl(65, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2022-10"
          type: text
      - condition: AND
        disabled: true
        label: "11月"
        color: "hsl(16, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2022-11"
          type: text
      - condition: AND
        disabled: true
        label: "12月"
        color: "hsl(208, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2022-12"
          type: text
```
