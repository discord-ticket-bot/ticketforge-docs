# Roles & Permissions

TicketForge divides permissions into two main categories: **Dashboard Access** and **Ticket Usage**.

## Dashboard Access

By default, only the **Server Owner** and users with the **Administrator** permission in Discord can access the web dashboard.

To grant access to other staff (e.g., "Head Moderator") without giving them full Administrator power:

1.  Go to **Server Config** in the dashboard.
2.  Find **Dashboard Access**.
3.  Select the roles you want to authorize.

<figure markdown>
  ![Roles Config](../assets/images/settings/roles-config.png){ loading=lazy }
  <figcaption>Selecting roles to grant dashboard access.</figcaption>
</figure>

!!! note "Access Level"
    Roles added here will have full access to edit Panels, Messages, and Settings for this specific server. They cannot access Billing or Subscription settings.

## Interaction Blacklist

If you have problematic users or roles that abuse the ticket system, you can blacklist them globally.

1.  Go to **Server Config**.
2.  Find **Interaction Blacklist**.
3.  Select the roles.

<figure markdown>
  ![Blacklist Config](../assets/images/settings/blacklist-roles-config.png){ loading=lazy }
  <figcaption>Preventing specific roles from interacting with the bot.</figcaption>
</figure>

**Effect:** Users with these roles cannot click _any_ button, use _any_ dropdown, or execute _any_ slash command associated with the bot.

## Bot Identity

You can customize how TicketForge appears specifically in your server, allowing it to match your server's theme or branding.

!!! example "Premium Feature"
    Changing the Bot Identity is a **Premium** feature.

1.  Go to **Server Config**.
2.  Find the **Bot Identity** card.

### Server Nickname
You can set a specific nickname for the bot in your server. This will change how the bot's name appears in the member list and in chat messages. 
Leaving this field blank will revert the bot to its default username.

### Server Avatar
You can upload a custom image (PNG, JPG, or GIF) to act as the bot's profile picture **only inside your server**. 
If you reset this, the bot will revert to its global Application Icon.

<figure markdown>
  ![Bot Identity Config](../assets/images/settings/bot-identity.png){ loading=lazy }
  <figcaption>Setting a custom nickname and avatar for the bot.</figcaption>
</figure>

## Server Language

You can change the language the bot uses for default system messages (e.g., errors, time formatting).

<figure markdown>
  ![Language Config](../assets/images/settings/language.png){ loading=lazy }
  <figcaption>Setting the bot's default language for the server.</figcaption>
</figure>

## Hierarchy Warning

For TicketForge to manage roles (e.g., adding/removing "Support" roles during claiming), the **TicketForge** bot role must be physically higher in the Discord Server Settings > Roles list than the roles it is trying to manage.