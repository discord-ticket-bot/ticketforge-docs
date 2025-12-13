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

## Role Access (Permissions)

TicketForge uses Discord's permission system to keep tickets private.

1.  **Opened Roles:** Select which roles should have access when a ticket is created (e.g., "Support Team", "Moderator").
2.  **Closed Roles:** Select roles that should be added or removed when a ticket is closed (e.g., allow "Admins" to see closed tickets but remove "Support Staff").

!!! warning "Permission Overwrites"
    The bot must have the **Manage Channels** permission to set these overwrites. Additionally, the bot's highest role must be above the roles you are trying to manage in the Discord Server Settings.

## Tickets as Threads (Premium)

Instead of creating a new Text Channel for every ticket, you can choose to create **Private Threads** inside a single parent channel.

- **Cleaner Channel List:** Keeps your sidebar organized.
- **Parent Channel:** Select a text channel where all threads will be spawned.
- **Permissions:** Thread permissions inherit from the parent channel, but TicketForge will invite the relevant staff members automatically if configured.