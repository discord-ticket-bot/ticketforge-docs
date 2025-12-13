# Creating Panels

A **Panel** is the interface your users interact with to open tickets. You can have multiple panels for different purposes (e.g., "Support", "Apply", "Report").

## Creating a New Panel

1. Go to the **Panels** tab in the dashboard sidebar.
2. Click the **Create Panel** card.
3. Choose a starting point:

### Method A: Use a Template

Choose from **Official** templates (created by the TicketForge team) or **Community** templates. Templates come pre-configured with message text, settings, and button styles.

- **Free Templates:** Available to everyone.
- **Premium Templates:** Include advanced features like Forms or Claiming enabled by default.

### Method B: Import Share Code

If you have a share code from another server (format: `XXXX-XXXX-XXXX`), select the **Import Code** tab. This will clone the exact configuration of that panel.

---

## Deploying to Discord

Once your panel is created and configured, you need to send it to a text channel in your server so users can see it.

1. Open the **Panel Editor**.
2. Locate the toolbar at the top of the settings area.
3. Click the **Send** button (Paper Plane icon).
4. Select the target channel from the dropdown list.
5. Click **Confirm**.

The bot will immediately post the panel message with the attached buttons or dropdown menu in Discord.

!!! tip "Updating Live Panels"
    If you change the text, color, or button style of a panel _after_ sending it, you do not need to delete and resend it.

    Simply click the **Update** button in the toolbar, paste the **Message Link** (Right-click message in Discord -> Copy Message Link), and the bot will edit the existing message in place.

## Managing Panels

In the Panel Editor toolbar, you also have access to:

- **Code:** Generate a share code to copy this panel to another server.
- **Clone:** Create an exact duplicate of the current panel within the same server.
- **Template:** Convert your panel into a public template for others to use.
