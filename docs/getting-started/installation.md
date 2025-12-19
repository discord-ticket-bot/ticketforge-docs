# Installation & Invite

Getting TicketForge running on your server takes just a few clicks.

## 1. Invite the Bot

To start using TicketForge, you need to invite the bot to your Discord server and authorize it with the necessary permissions.

<div class="grid cards" markdown>

- :fontawesome-brands-discord: **Invite TicketForge**<br>
  Click below to add the bot to your server. You must have **Manage Server** permissions.<br>
  [:fontawesome-brands-discord: Invite Bot](https://discord.com/oauth2/authorize?client_id=1312832688889008218&permissions=361046076432&integration_type=0&scope=bot){ .md-button .md-button--primary }

</div>

<figure markdown>
  ![Invite Screen](../assets/images/getting-started/invite-screen.png){ loading=lazy width="450" }
  <figcaption>The Discord authorization screen when inviting the bot.</figcaption>
</figure>

## 2. Required Permissions

TicketForge requires specific permissions to function correctly. When inviting the bot, ensure the following permissions are granted:

| Permission | Reason |
| :--- | :--- |
| **Manage Roles** | To assign support roles, manage ticket permissions, and automate roles during claiming. |
| **Manage Channels** | To create ticket channels, rename them, and manage categories. |
| **View Channels** | Essential for the bot to see and interact with your server's channels. |
| **Send Messages** | To post panels, welcome messages, and response triggers inside tickets. |
| **Send Messages in Threads** | Required if you use the "Tickets as Threads" Premium feature. |
| **Create Private Threads** | Allows the bot to create private ticket threads for a cleaner sidebar (Premium). |
| **Manage Messages** | To pin messages and delete bot triggers/commands to keep channels clean. |
| **Embed Links** | Necessary to send rich visual panels, buttons, and formatted logs. |
| **Attach Files** | Used to generate and upload HTML transcripts and audit logs. |
| **Read Message History** | Required to generate transcripts and view context of existing tickets. |
| **Use External Emojis** | Allows the bot to display custom branding and icons in its messages. |

!!! warning "Permission Check"
    Ensure the TicketForge bot role is higher than the roles you select below in your server settings. 

    For TicketForge to manage roles (e.g., adding a "Support" role to a user), the **TicketForge bot role** must be **higher** than the role it is trying to assign in your Discord Server Settings > Roles list.

## 3. Verify Installation

Once invited, go to a text channel in your server and type `/ping`.
If the bot responds with **"🏓 Pong!"**, it is successfully installed and online.

---

## Troubleshooting

**The bot is offline?**
Check our [Status Page](https://ticketforge.statuspage.io/) to see if there are any ongoing outages.

**Commands not showing up?**
Sometimes Discord takes up to an hour to register slash commands for new bots. You can try re-inviting the bot with the link above to force a command refresh.