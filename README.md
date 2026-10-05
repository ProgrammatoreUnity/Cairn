# CAIRN

**Designer software to keep your mind focused on building your project.**

[Versione italiana](README.it.md)

Cairn is a Windows app that keeps everything about a project in one place: the tasks to do, the plan over time, your sketches and your notes. It works completely offline. There is no cloud, no server and no online account, so your work stays on your PC.
Warning: Part of the README was written by AI and may contain translation errors.

## Getting started

1. Run `Cairn.exe`. There is nothing to install.
2. Create your account. It is stored only on this PC and is used to show who did what.
3. Click **New Project**, give it a name, and open it with a double-click.

Everything you do is saved automatically. There is no Save button to remember.

## The main menu

The first screen is your list of projects. From here you can create a project, open one, change its settings, or delete it.

**Open Folder…** adds a project that already exists on your disk, for example one a teammate shared with you.

## Inside a project

A project has three areas. Switch between them from the top of the window or from the **View** menu.

### Kanban board

The board shows your tasks as cards, arranged in columns such as *TODO*, *In Progress* and *Done*.

- Add a card for each thing to do.
- Drag a card to another column when its status changes.
- Add, rename, recolor or remove columns to match the way you work.
- Send finished cards to the **archive** to keep the board tidy.

Open a card to add details:

- a description, an assignee, a priority and tags
- a checklist and subtasks, with a circle showing how much is done
- dates: when it starts, when it is due, when it finished
- comments
- links to documents of the project

A card also keeps a history of its changes. Changes to a card are applied only when you press **Save**.

Use the filters and the search box to see only the cards you care about, for example only yours or only the urgent ones. Cairn also tells you when a task is overdue or close to its deadline.

### Roadmap

The roadmap opens in its own window and shows your tasks on a timeline, so you can see what happens when.

- Tasks that have dates appear as bars, grouped by tag.
- Add **milestones** to mark important moments, each with its own icon.
- Add tasks that live only on the roadmap.
- Look at a single month, a whole year, or zoom freely from 7 days to 2 years.

### Whiteboard

A free space to draw ideas and connect them.

- Add shapes, text, drawings and images, then join them with connectors.
- Link an element to a task or a document.
- Mark the important elements as favorites.
- Create as many whiteboards as you need in a project.
- Undo and redo are always available.

### Documentation

The place for the written part of your project.

- Write simple **Markdown** notes or formatted **Rich Text** pages with fonts, colors, lists and images.
- Organize documents in folders.
- Link documents to each other. The **graph view** shows how they are connected.
- A deleted document goes to the project's trash folder. Cairn never empties it by itself.

### Pomodoro timer

A timer at the top of the window helps you work in focused sessions with short breaks. Each project has its own timer settings.

## Where your data lives

Each project is a normal folder on your disk, made of readable files.

- **Backup:** copy the folder.
- **Share:** send the folder, or keep it in Git and share it with your team.
- **Safety net:** Cairn keeps the last 5 automatic backups of each board. You can restore one from the project settings.

## Accounts

Accounts are local and need no internet. Passwords are stored encrypted. Several people can use Cairn on the same PC, each with their own account, name and picture. Cairn remembers you on your PC, and you can log out or switch account from the menu at the top right.

## Light and dark

Switch between the light and the dark theme with the sun/moon button at the top right.

## Good to know

- Editing a Markdown document in preview mode rewrites it in Cairn's own Markdown style.
- Converting a Rich Text page to Markdown loses colors, fonts and alignment.
- Rich Text pages with many images can feel slow while typing.
- A link to an external file stops working if that file is moved.

## Requirements

Windows, 64-bit.

## Credits

Designed and realized by Highshore Studio - highshore.studio@gmail.com

Milestone icons: [Ionicons](https://ionic.io/ionicons) (MIT license).
