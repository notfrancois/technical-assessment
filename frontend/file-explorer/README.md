# Frontend File Explorer Exercise

## Overview

Given an array of file objects, build a component that displays them in a hierarchical tree format.

There are two types of objects – files and directories:

1.  Files are essentially leaf nodes of the tree, they do not have children.
2.  Directories can contain other objects – either files or directories.

You may assume that the IDs and names within the same directory are unique.

## Requirements

1.  The names of the directories/files should be displayed.
2.  Directories
    -   Contents of the directory should be displayed in a manner that indicates it belongs within the directory. The recommended approach is to indent the contents to the right.
    -   Directories can be expanded and collapsed. Clicking on a directory should toggle its expanded/collapsed state.
    -   Directories should appear before files. All the items should be sorted alphabetically within their respective categories.
    -   You may style the expand/collapse functionality in a way you prefer as long as it is clear that the item is a directory and whether it is in the expanded or collapsed state.
    -   Directories can be empty.
3.  Files
    -   Files are not expandable and cannot be interacted with.
    -   The focus of the exercise is on the functionality and not the styling.

## Data Format

The data is given in the following format:

```ts
interface FileObject {
	id: number;
	name: string;
	children?: FileObject[];
}
```

## Example

```ts
const fileData = [
	{
		id: 1,
		name: "README.md",
	},
	{
		id: 2,
		name: "Documents",
		children: [
			{
				id: 3,
				name: "Word.doc",
			},
			{
				id: 4,
				name: "Powerpoint.ppt",
			},
		],
	},
];
```

## Plus Points

-   Implement a "Reset" button to reset the file explorer.
-   Implement a "Collapse All" button to collapse all the directories.
-   Implement a "Expand All" button to expand all the directories.
-   Use beautiful icons to indicate the type of the file.
