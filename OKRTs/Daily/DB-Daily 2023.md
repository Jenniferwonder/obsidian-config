---

database-plugin: basic

---

```yaml:dbfolder
name: DB-Daily-2023
description: new description
columns:
  column1:
    input: text
    key: column1
    accessorKey: column1
    label: Column 1
    position: 2
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
    position: 1
    isHidden: false
    sortIndex: 1
    isSorted: true
    isSortedDesc: true
    width: 68
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
    width: 257
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
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
    position: 31
    isHidden: false
    sortIndex: -1
    width: 221
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
    id: Title
    label: Title
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 97
    config:
      enable_media_view: false
      link_alias_enabled: false
      media_width: 100
      media_height: 100
      isInline: false
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
    position: 17
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
  EveningExercise:
    input: checkbox
    accessorKey: EveningExercise
    key: EveningExercise
    id: EveningExercise
    label: EveningExercise
    position: 19
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
  Aerobics:
    input: checkbox
    accessorKey: Aerobics
    key: Aerobics
    id: Aerobics
    label: Aerobics
    position: 20
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
  Strength:
    input: checkbox
    accessorKey: Strength
    key: Strength
    id: Strength
    label: Strength
    position: 21
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
  __inlinks__:
    key: __inlinks__
    id: __inlinks__
    input: inlinks
    label: Inlinks
    accessorKey: __inlinks__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: false
    position: 32
    isHidden: false
    sortIndex: -1
    width: 296
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
    position: 27
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
  TechSkills:
    input: text
    accessorKey: TechSkills
    key: TechSkills
    id: TechSkills
    label: TechSkills
    position: 9
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
  PMP:
    input: text
    accessorKey: PMP
    key: PMP
    id: PMP
    label: PMP
    position: 12
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
  PKM:
    input: text
    accessorKey: PKM
    key: PKM
    id: PKM
    label: PKM
    position: 11
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
  CPE:
    input: text
    accessorKey: CPE
    key: CPE
    id: CPE
    label: CPE
    position: 30
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
  Life:
    input: text
    accessorKey: Life
    key: Life
    id: Life
    label: Life
    position: 29
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
  ToImprove:
    input: text
    accessorKey: ToImprove
    key: ToImprove
    id: ToImprove
    label: ToImprove
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 100
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
  Coding:
    input: checkbox
    accessorKey: Coding
    key: Coding
    id: Coding
    label: Coding
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
  Act:
    input: checkbox
    accessorKey: Act
    key: Act
    id: Act
    label: Act
    position: 33
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
  Revision:
    input: checkbox
    accessorKey: Revision
    key: Revision
    id: Revision
    label: Revision
    position: 14
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
  MoneySpent:
    input: number
    accessorKey: MoneySpent
    key: MoneySpent
    id: MoneySpent
    label: MoneySpent
    position: 28
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
  Weight:
    input: number
    accessorKey: Weight
    key: Weight
    id: Weight
    label: Weight
    position: 23
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
  Anki:
    input: checkbox
    accessorKey: Anki
    key: Anki
    id: Anki
    label: Anki
    position: 13
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
  Dance:
    input: checkbox
    accessorKey: Dance
    key: Dance
    id: Shape
    label: Dance
    position: 22
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
  Food:
    input: number
    accessorKey: Food
    key: Food
    id: Food
    label: Food
    position: 24
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
  Transport:
    input: number
    accessorKey: Transport
    key: Transport
    id: Transport
    label: Transport
    position: 25
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
  Growth:
    input: number
    accessorKey: Growth
    key: Growth
    id: Growth
    label: Growth
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
  Stretch:
    input: checkbox
    accessorKey: Stretch
    key: Stretch
    id: MorningExercise
    label: Stretch
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
  StudyTime:
    input: number
    accessorKey: StudyTime
    key: StudyTime
    id: StudyTime
    label: StudyTime
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 42
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
  GymTime:
    input: number
    accessorKey: GymTime
    key: GymTime
    id: GymTime
    label: GymTime
    position: 8
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
  Location:
    input: tags
    accessorKey: Location
    key: Location
    id: Location
    label: Location
    position: 10
    skipPersist: false
    isHidden: true
    sortIndex: -1
    options:
      - { label: "Lib,Gym", value: "Lib,Gym", color: "hsl(13, 95%, 90%)"}
      - { label: "Lib", value: "Lib", color: "hsl(302, 95%, 90%)"}
      - { label: "Gym", value: "Gym", color: "hsl(208, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Reading:
    input: checkbox
    accessorKey: Reading
    key: Reading
    id: Reading
    label: Reading
    position: 15
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
  WakeUp:
    input: text
    accessorKey: WakeUp
    key: WakeUp
    id: WakeUp
    label: WakeUp
    position: 6
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
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: true
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: true
  show_metadata_inlinks: true
  show_metadata_outlinks: true
  show_metadata_tags: false
  source_data: tag
  source_form_result: "#Daily"
  source_destination_path: 000-OKRTs/Daily
  row_templates_folder: /
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
        color: "hsl(358, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-01"
          type: text
      - condition: AND
        disabled: true
        label: "2月"
        color: "hsl(24, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-02"
          type: text
      - condition: AND
        disabled: true
        label: "3月"
        color: "hsl(58, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-03"
          type: text
      - condition: AND
        disabled: true
        label: "4月"
        color: "hsl(254, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-04"
          type: text
      - condition: AND
        disabled: true
        label: "5月"
        color: "hsl(304, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-05"
          type: text
      - condition: AND
        disabled: true
        label: "6月"
        color: "hsl(201, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-06"
          type: text
      - condition: AND
        disabled: false
        label: "7月"
        color: "hsl(4, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-07"
          type: text
      - condition: AND
        disabled: true
        label: "8月"
        color: "hsl(115, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-08"
          type: text
      - condition: AND
        disabled: true
        label: "9月"
        color: "hsl(211, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-09"
          type: text
      - condition: AND
        disabled: true
        label: "10月"
        color: "hsl(189, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-10"
          type: text
      - condition: AND
        disabled: true
        label: "11月"
        color: "hsl(122, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-11"
          type: text
      - condition: AND
        disabled: true
        label: "12月"
        color: "hsl(72, 95%, 90%)"
        filters:
        - field: file.name
          operator: CONTAINS
          value: "2023-12"
          type: text
```