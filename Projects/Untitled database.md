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
    width: -49
    config:
      enable_media_view: true
      link_alias_enabled: true
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
    position: 4
    isHidden: false
    sortIndex: -1
    width: 161
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
    label: started
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
  due:
    input: calendar
    accessorKey: due
    key: due
    id: due
    label: due
    position: 8
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
  tags:
    input: tags
    accessorKey: tags
    key: tags
    id: tags
    label: tags
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 245
    options:
      - { label: "Projects/Miniprogram", value: "Projects/Miniprogram", color: "hsl(247, 95%, 90%)"}
      - { label: "Projects/Mobile-App", value: "Projects/Mobile-App", color: "hsl(202, 95%, 90%)"}
      - { label: "Front-End", value: "Front-End", color: "hsl(30, 95%, 90%)"}
      - { label: "PMP", value: "PMP", color: "hsl(173, 95%, 90%)"}
      - { label: "Projects/PWA", value: "Projects/PWA", color: "hsl(3, 95%, 90%)"}
      - { label: "moc", value: "moc", color: "hsl(224, 95%, 90%)"}
      - { label: "Projects/Admin", value: "Projects/Admin", color: "hsl(262, 95%, 90%)"}
      - { label: "Projects/Documentation", value: "Projects/Documentation", color: "hsl(276, 95%, 90%)"}
      - { label: "Projects/Low-Code", value: "Projects/Low-Code", color: "hsl(13, 95%, 90%)"}
      - { label: "Projects/Content Editor", value: "Projects/Content Editor", color: "hsl(301, 95%, 90%)"}
      - { label: "Projects/Game", value: "Projects/Game", color: "hsl(195, 95%, 90%)"}
      - { label: "React", value: "React", color: "hsl(4, 95%, 90%)"}
      - { label: "GeekEnglish/Plans", value: "GeekEnglish/Plans", color: "hsl(90, 95%, 90%)"}
      - { label: "Projects/GeekEnglish/Plans", value: "Projects/GeekEnglish/Plans", color: "hsl(275, 95%, 90%)"}
      - { label: "GeekEnglish/Functions", value: "GeekEnglish/Functions", color: "hsl(40, 95%, 90%)"}
      - { label: "Projects/GeekEnglish/Design", value: "Projects/GeekEnglish/Design", color: "hsl(348, 95%, 90%)"}
      - { label: "GeekEnglish/Setup", value: "GeekEnglish/Setup", color: "hsl(173, 95%, 90%)"}
      - { label: "GeekEnglish/System", value: "GeekEnglish/System", color: "hsl(309, 95%, 90%)"}
      - { label: "GeekEnglish/Workflow", value: "GeekEnglish/Workflow", color: "hsl(15, 95%, 90%)"}
      - { label: "GeekEnglish/Logs", value: "GeekEnglish/Logs", color: "hsl(233, 95%, 90%)"}
      - { label: "GeekEnglish/Related/Portfolio", value: "GeekEnglish/Related/Portfolio", color: "hsl(177, 95%, 90%)"}
      - { label: "GeekEnglish/Related", value: "GeekEnglish/Related", color: "hsl(212, 95%, 90%)"}
      - { label: "Projects/TechBlog", value: "Projects/TechBlog", color: "hsl(23, 95%, 90%)"}
      - { label: "Projects/Medium-Clone", value: "Projects/Medium-Clone", color: "hsl(211, 95%, 90%)"}
      - { label: "Projects/Twitter-Clone", value: "Projects/Twitter-Clone", color: "hsl(122, 95%, 90%)"}
      - { label: "Projects/E-Commerce", value: "Projects/E-Commerce", color: "hsl(133, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  OKR:
    input: text
    accessorKey: OKR
    key: OKR
    id: OKR
    label: OKR
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 155
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
    label: status
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "🟡Organizing", value: "🟡Organizing", color: "hsl(235, 95%, 90%)"}
      - { label: "⚪Capturing", value: "⚪Capturing", color: "hsl(346, 95%, 90%)"}
      - { label: "🔵Archived", value: "🔵Archived", color: "hsl(189, 95%, 90%)"}
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
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
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
  enabled: false
  conditions:
```