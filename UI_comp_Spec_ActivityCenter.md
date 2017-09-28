# UI Component [Activity Center] V1.0
### Usage
- View all notifications
- Sort notifications into read and unread categories 
- Lead user to the corresponded details page

### UI Elements
- **Actionbar**:
  - Title: Activity
- **Tapbar**:
  - Button: Unread
  - Button: Read
- **ListView**:
  - ListUnread: Unread notification items 
  - ListRead: Read notification items 
  - ListItem: 
    - Subject thumbnail on the left end
    - Content preview thumbnail/icon on the right end
    - Subject title
    - Time stamp
    - Content description brief
    - Unread item will be highlighted
    - Items display in an reversed chronological order
 
### Behaviors 
- **Tapbar_Unread {Tap} :**
  - Display the unread notification list
- **Tapbar_Read {Tap} :**
  - Display the read notification list
- **ListView_ListItem {Tap} :**
  - Lead to corresponded details page
  - When and only when an unread item been tapped, it will turn into Read status, the Unread highlight disappeares
- **ListView_ListView {Scroll} :**
  - When the list view is already scrolled to the top, pull down the list further the view will be refreshed

### Wireframes
[Activity Center Unread View](https://www.jianguoyun.com/p/DRF4Ta4QpqzHBhj9hjY)

[Activity Center Read View](https://www.jianguoyun.com/p/DfBXVRQQpqzHBhiAhzY)
