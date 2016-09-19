# Shaman.WinForms.IconHandler

Provides access to Windows Shell icons for file types.

```csharp
using Shaman.WinForms;

// Standalone usage
Image img = IconHandler.GetIcon(".zip", true, false);

// Usage in a ListView
var iconHandler = new IconHandler(true, true);
listView.SmallImageList = iconHandler.SmallIcons;

listViewItem1.ImageIndex = iconHandler.GetIcon(".zip");

```