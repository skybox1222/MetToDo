# MetToDo

A simple, clickable to-do list skin for [Rainmeter](https://www.rainmeter.net/) (Windows 10/11).

![Screenshot] <img width="481" height="374" alt="105304" src="https://github.com/user-attachments/assets/1c8dc032-29fa-4bb2-beff-a14f4c30010b" />


## Features

- Task list with a checkbox next to each title
- Click the checkbox to mark a task as done (the box fills, the text is struck through and changes color). Click again to undo
- `+` to add a task, click the title (or Edit) to rename it, Del to remove it
- The skin resizes itself to the number of tasks
- Completed tasks are logged with date and time in `done.log`
- Fonts, sizes and colors are fully customizable

## Installation

1. Download `MetToDo_1_0.rmskin` from the [Releases](../../releases) page.
2. Double-click it and click **Install**.
3. If the skin doesn't load by itself, open Rainmeter, go to the **ToDo** folder and load `TodoList.ini`.

Requires Rainmeter 4.5 or newer.

## Usage

| Action | How |
| --- | --- |
| Add a task | Click `+`, type, press Enter |
| Edit a task | Click its title or **Edit**, change the text, press Enter |
| Complete / undo | Click the checkbox |
| Delete a task | Click **Del** |
| Edit the list by hand | Right-click the skin, then "Modifica lista a mano (todo.txt)" |
| Reload | Right-click the skin, then "Reload" |

Tasks are stored in `todo.txt`, one per line. Lines starting with `[x] ` are completed tasks.

## Customization

Right-click the skin and choose "Modifica colori e font" to open `Settings.inc`. You can change:

- font face and size for tasks, title and icons
- colors for background, text, accent, icons and completed tasks (text and checkbox border)
- width, row height, checkbox size and corner radius

Save the file and refresh the skin.

## Notes

- **Do not enable "Click through"** in the Rainmeter skin settings, otherwise the checkboxes and buttons won't respond.
- Some labels (context menu entries and the empty-list message) are in Italian. You can change them in `TodoList.ini` and `todo.lua`.
- The input box doesn't accept text containing `]]`.
- A task that starts with `[x]` is read as already completed.
- Updating the skin by installing a new package may overwrite your skin files: back up `todo.txt` first.

## License

MIT
