# Collapsible Sidebar

## Overview
The **Collapsible Sidebar** component is a customizable sidebar for applications that can expand and collapse. It is designed for flexibility, allowing you to control its appearance and behavior through a variety of properties.

## Features
- **Expandable and Collapsible**: Toggle the sidebar's visibility to maximize screen real estate.
- **Customizable Menu**: Display various menu items with icons and text.
- **Responsive Design**: The sidebar's width adjusts based on the application's width and whether it is expanded or collapsed.
- **Consistent Styling**: Customize colors, padding, fonts, and other styling properties to match your application's theme.

## Properties

| Property             | Type   | Description                                                        |
|----------------------|--------|--------------------------------------------------------------------|
| SidebarIconSize      | Number | Controls the size of icons within the sidebar.                     |
| SidebarMenuTable     | Table  | Defines the menu items displayed in the sidebar. **Note:** The structure of data in `SidebarMenuTable` should not be altered. |
| SidebarPadding       | Number | Sets the padding around the content within the sidebar.            |
| SidebarPrimaryColor  | Color  | The primary color of the sidebar (e.g., background color).         |
| SidebarSecondaryColor| Color  | The secondary color of the sidebar (e.g., text color).             |
| SidebarPrimaryFont   | String | The font used for text within the sidebar.                         |
| SidebarWidth         | Number | The width of the sidebar, which adjusts dynamically based on whether it is expanded or collapsed. |
| SidebarSelectedText  | String | The text output of the selected menu item.                         |

## Usage

1. **Toggle Sidebar Visibility**:
   - The sidebar can be expanded or collapsed using a toggle button, which changes the state of `isSidebarExpanded`.
  
2. **Menu Items**:
   - The sidebar menu is defined by the `SidebarMenuTable` property, which allows you to specify a list of menu items. Each item can have an associated icon, text, and output value.
  
3. **Styling**:
   - The appearance of the sidebar is highly customizable. You can adjust the `SidebarPrimaryColor`, `SidebarSecondaryColor`, `SidebarPrimaryFont`, and `SidebarPadding` to fit your design requirements.

4. **Event Handling**:
   - The `OnSelect` property of the toggle button manages the sidebar's expansion state. Similarly, the `OnSelect` property of each menu item can be used to trigger specific actions when the item is clicked.

## Example

```yaml
CollapsibleSidebar:
  SidebarIconSize: 52
  SidebarMenuTable: Table(
      { Icon: Icon.Home, Text: "Home", Output: "Home" },
      { Icon: Icon.Mail, Text: "Message", Output: "Message" },
      { Icon: Icon.Settings, Text: "Config", Output: "Config" },
      { Icon: Icon.Person, Text: "Profile", Output: "Profile" },
      { Icon: Icon.Leave, Text: "Logout", Output: "Logout" }
  )
  SidebarPadding: 12
  SidebarPrimaryColor: RGBA(31, 41, 55, 1)
  SidebarSecondaryColor: Color.White
  SidebarPrimaryFont: App.Theme.Font
  SidebarWidth: App.Width * 0.2
  SidebarSelectedText: ""
```

## Customization
- **Adding Menu Items**: Extend the `SidebarMenuTable` by adding new menu items with custom icons and text.
- **Styling Adjustments**: Modify the `SidebarPrimaryColor`, `SidebarSecondaryColor`, and `SidebarPrimaryFont` to align with your application's theme.
- **Behavior Control**: Adjust the `OnSelect` events in the sidebar's toggle button and menu items to customize interactions.

This component is ideal for applications that require a dynamic and customizable navigation interface.