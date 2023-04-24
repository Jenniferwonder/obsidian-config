---
sorting-spec: |
 //
 // A simple configuration for obsidian-custom-sort plugin
 // (https://github.com/SebastianMC/obsidian-custom-sort)
 // It causes the plugin to take over the control of the order of items in the root folder ('/') of the vault
 // It explicitly sets the sorting to descending ('>') alphabetical ('a-z')
 // Folders and files are treated equally by the plugin (by default) so expect them intermixed
 // in the root vault folder after enabling the custom sort plugin
 // 
 // To play with more examples go to https://github.com/SebastianMC/obsidian-custom-sort#readme

 target-folder: /*
 < a-z
 
 target-folder: Front-End Projects
 ...
 < a-z 
 target-folder: PKM
 < a-z
 target-folder: Programming-Fundamentals
 < a-z 
 target-folder: 01-Inbox/Daily
 > a-z
---
