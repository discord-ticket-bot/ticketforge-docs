# Transcripts & Logging

TicketForge provides robust record-keeping features to ensure you never lose context of a support interaction, even after the ticket is deleted.

## Transcript Archiving

A transcript is a permanent HTML file containing the full chat history, timestamps, and attachments of a ticket.

### Configuration

Navigate to **Archiving & Logging** in the Panel Editor.

1.  **Storage Channel:** Select a text channel in your server where the bot will post the transcript files.
2.  **Auto-Save:** automatically generate a transcript when a ticket is closed.
    - _Trigger:_ Choose whether to save on **Close** (archive state) or **Delete** (permanent removal).
3.  **DM Transcript:** Send the HTML file directly to the user who opened the ticket.
    - _Note:_ This will fail if the user has Direct Messages disabled.

## Event Audit Log

Separate from message history, the Event Log tracks the _lifecycle_ of the ticket.

### Setup

1.  **Audit Log Channel:** Select a channel to receive real-time embed updates.
2.  **Events:** Toggle which specific actions trigger a log message:

| Event        | Trigger                                |
| :----------- | :------------------------------------- |
| **Created**  | A user successfully opens a ticket.    |
| **Closed**   | Staff or user clicks the Close button. |
| **Reopened** | A closed ticket is re-opened.          |
| **Renamed**  | The channel name is changed via bot.   |
| **Deleted**  | The channel is permanently deleted.    |
| **Archived** | A transcript file is generated.        |

### Log Content

The log embed includes:

- Ticket ID and Panel Name.
- The User (Target) and the Executor (Staff member).
- Reason (if provided).
- Timestamp.
