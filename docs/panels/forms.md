# Ticket Forms

Forms allow you to collect specific information from a user _before_ the ticket is created. When a user clicks the "Create Ticket" button, a modal appears asking for details.

## Configuration

1.  Navigate to the **Ticket Forms** tab in the Panel Editor.
2.  Toggle **Enable Ticket Forms** to ON.

### Adding Questions

You can add multiple questions to gather context (e.g., "Minecraft Username", "Reason for Report", "Device ID").

| Option             | Description                                                          |
| :----------------- | :------------------------------------------------------------------- |
| **Label**          | The question text shown to the user (e.g., "What is your ign?").     |
| **Placeholder**    | Greyed-out text inside the box to guide the user.                    |
| **Required**       | If enabled, the user cannot submit the form without answering.       |
| **Multi-line**     | Switches the input from a single line to a paragraph text area.      |
| **Min/Max Length** | Enforce character limits to prevent spam or ensure detailed answers. |

### Results

Once submitted, the answers are automatically compiled into an embed field and posted as the first message inside the newly created ticket.

![Form Preview](../assets/images/form-preview.png){ align=right width=300 }
_A preview of how the form looks in Discord._
