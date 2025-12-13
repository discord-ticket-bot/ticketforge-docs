# Command Management

TicketForge offers granular control over Slash Commands. You can disable specific commands entirely or restrict them to specific channels and roles.

## Configuration

Navigate to the **Commands** tab in the sidebar. You will see a list of all available bot commands.

<figure markdown>
  ![Commands List](../assets/images/settings/commands-list.png){ loading=lazy }
  <figcaption>The command management interface allowing you to enable or disable specific commands.</figcaption>
</figure>

### Command Settings

Click on any command to edit its permissions:

1.  **Enable Command:** Master toggle. If OFF, the command acts as if it doesn't exist.
2.  **Support Team Only:** Restricts usage to users who have a role designated as "Support" in any of your panels.
    - _Admin Commands (e.g., `/setup`, `/purge-tickets`) are restricted to Administrators automatically._

### Scope Restrictions

You can fine-tune where commands work:

- **Allowed Channels:** The command will _only_ work in these channels.
- **Blocked Channels:** The command will work everywhere _except_ these channels.
- **Allowed Roles:** Only these roles can use the command.
- **Blocked Roles:** These roles are specifically prevented from using the command.

## Available Commands

| Command               | Description                                                                         |
| :-------------------- | :---------------------------------------------------------------------------------- |
| **General**           |                                                                                     |
| `/help`               | Displays the help menu with a list of available commands.                           |
| `/ping`               | Checks bot latency and API response time.                                           |
| `/invite`             | Provides the link to invite TicketForge to other servers.                           |
| `/premium`            | Shows the current server subscription tier and expiry date.                         |
| **Ticket Management** |                                                                                     |
| `/close`              | Closes the current ticket (triggers the Close logic configured in the panel).       |
| `/claim`              | Assigns the ticket to the user running the command.                                 |
| `/unclaim`            | Releases the ticket back to the general pool.                                       |
| `/add <user/role>`    | Adds a specific user or an entire role to the current ticket.                       |
| `/remove <user/role>` | Removes a specific user or role from the current ticket.                            |
| `/rename <name>`      | Renames the current ticket channel.                                                 |
| `/priority`           | Sets the priority level of the ticket (Low, Medium, High, Urgent).                  |
| **Admin**             |                                                                                     |
| `/setup`              | Launches the interactive setup wizard for creating panels directly in Discord.      |
| `/purge-tickets`      | Opens a menu to bulk delete tickets based on their status (All Open or All Closed). |