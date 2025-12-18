# Ticket Management

This section controls the structural behavior of the tickets created by this panel: where they go, what they are named, and who can see them.

<figure markdown>
  ![Management Overview](../assets/images/panels/management-overview.png){ loading=lazy }
  <figcaption>Configuring channel naming, categories, and role access.</figcaption>
</figure>

## Channel Naming

You can define a naming pattern for your tickets.

- **Default:** `ticket-{count}`
- **Variables:**
  - `{user}` - The username of the ticket creator.
  - `{count}` - The unique ticket number.
  - `{panel.name}` - The name of the panel.

## Role Automation

TicketForge can automatically give or take away roles from a user depending on whether their ticket is open or closed. This is perfect for keeping your member list organized or giving temporary access while a ticket is active.

### Ticket Opened

- **Add Roles:** Select roles that should be automatically given to the user the moment they open a ticket. This is useful for tagging users with a "Currently in Support" role.
- **Remove Roles:** Automatically strip roles from the user when the ticket is created 

### Ticket Closed

When a ticket is closed, you can clean up roles or add new ones:

- **Add Roles:** Give the user a specific role once their ticket is closed (e.g., a "Ticket History" role).
- **Remove Roles:** Automatically strip roles from the user when the ticket is closed (e.g., removing the "Active Ticket" role you gave them at the start).

!!! tip "Staff Access"
    If you are looking to set who can **view and reply** to the tickets, you should set your **Support Team** roles in the "General & Quickedit" section of the panel editor.

!!! warning "Permission Overwrites"
    The bot must have the **Manage Channels** permission to set these overwrites. Additionally, the bot's highest role must be above the roles you are trying to manage in the Discord Server Settings.

## Internal Staff Threads (Premium)

When a ticket is opened, TicketForge can automatically create a private thread inside the ticket channel. This is a dedicated space where your staff can discuss the case or take notes without the user ever seeing the messages.

- **Private Discussions:** Keep internal coordination, evidence, or staff-only notes hidden from the ticket opener.
- **Auto-Invite:** TicketForge automatically invites your configured Support Team to the thread so they don't have to manually join.
- **Cleaner Logs:** Keeps the main ticket channel focused on the conversation with the user, while the "behind the scenes" talk stays in the thread.

!!! note "Visibility"
    Because this is a Discord thread inside the ticket channel, it will automatically be deleted whenever the main ticket channel is closed or deleted.