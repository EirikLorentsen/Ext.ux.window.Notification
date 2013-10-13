
# Notification extension for Ext JS 4.x (version: 2.1.2)

[**Examples and instructions**](http://www.eirik.net/Ext/ux/window/Demo.html)

New improved features include:
- Multiple managers and notifications stacks
- The static manager object is eliminated completely, allowing notifications to attach to different components using their x and y coordinates to slide in the notifications.
- All eight corners and edges of document/manager can be used: 'tl', 'tr', 'br', 'bl', 't', 'l', 'b', 'r'.
- Both x and y axis can be used on corners. Notifications can slide in sideways.
- When a notification is closed any notifications above it slide down automatically.
- Hovering the mouse over the notification delays auto closing.
- Easy customization of css, animations, delays, spacings/padding etc.

## License

Copyright (c) 2011 Eirik Lorentsen - http://www.eirik.net/

Based on the Ext.ux.Notification plugin by efattal.

Dual licensed under the MIT (http://www.opensource.org/licenses/mit-license.php) 
and GPL (http://www.opensource.org/licenses/gpl-license.php) licenses.

## Changelog:

### 2.1.3

- (anotheri) Bugfix: Notification destroys properly on close()

### 2.1.2

- (Brian428) Bugfix: Specifying origin x and y coordinates in the initial animation to avoid irregular animation. 

### 2.1.1

- Bugfix: Compatible with Ext JS 4.0.7
- Bugfix: Simplified hide function using fadeOut() eliminating some small snags

### 2.1

- Renamed autoHide to autoClose
- (Dmurat) Enabled reuse of notifications (closeAction: 'hide')
- (Idonofrio) Destroying notification by default (closeAction: 'destroy')

### 2.0 (2012-03-06)

http://www.eirik.net/Ext/ux/window/tags/Notification/2.0/Notification.js

- Renamed some properties ending with "Delay" to the more correct: "Duration".
- Moved the hiding animation out of destruction and into hide.
- Renamed the corresponding "destroy" properties to "hide".
- (Hpsam) Changed addClass to addCls.
- (Hpsam) Avoiding setting 'notification-fixed' when auto hiding.
- (Justmyhobby) Using separate arrays to enable managers to mix alignments.
- (Kreeve_ctisn) Removed default title.
- (Jmaia) Center of edges can be used for positioning. Renamed corner property to position.
- (Hpsam) Hiding or destroying manager does not cause errors.

### 1.3 (2011-09-13)

http://www.eirik.net/Ext/ux/window/tags/Notification/1.3/Notification.js

- Cleaned up component destruction

### 1.2 (2011-09-12)

http://www.eirik.net/Ext/ux/window/tags/Notification/1.2/Notification.js

- Added config options: stickOnClick and stickWhileHover.

### 1.1 (2011-09-01)

http://www.eirik.net/Ext/ux/window/tags/Notification/1.1/Notification.js

- Bugfix. Array.indexOf not universally implemented, causing errors in IE<=8. Replaced with Ext.Array.indexOf.