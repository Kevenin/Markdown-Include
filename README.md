# Markdown Include

[![Marketplace Version](https://vsmarketplacebadge.apphb.com/version-short/Kevenin.markdowninclude.svg)](https://marketplace.visualstudio.com/items?itemName=Kevenin.markdowninclude)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/Kevenin.markdowninclude.svg)](https://marketplace.visualstudio.com/items?itemName=Kevenin.markdowninclude)
[![Rating](https://vsmarketplacebadge.apphb.com/rating/Kevenin.markdowninclude.svg)](https://marketplace.visualstudio.com/items?itemName=Kevenin.markdowninclude)


This extention is used to merge Markdown files from various locations to one file.

## Features

- Merge single active md file using the MdMerge command. the file must include the following lines:
  - !import[/path/from/root/import.md] can be anywhere in the file
  - !export[/path/from/root/export.md] **MUST BE** the last line
- Merge all files from select folders using the MdMergeAll command
  - Add the folders in your workspaces settings.json
  ```json
  {
      "MdMerge.FolderPaths": [ "/ToPublish" ]
  }
  ```
  - Run the command from anywhere in your workspace

## Extension Settings

This extension contributes the following settings:

* `MdMerge.FolderPaths`: Contains the list of folders to go through with the MdMergeAll command

## Examples
For more detailed examples, please look at the [Markdown Test Files folder](https://github.com/Kevenin/Markdown-Include/tree/master/Markdown%20Test%20Files). It contains examples for both MdMerge and MdMergeAll.

## Change Log
See Change Log [here](CHANGELOG.md)
