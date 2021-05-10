# Reading 37 Notes

[Home](README.md)

# Xamarin: Data Services

Xamarin.Forms code runs on several different platforms and each have its own file system. Mobile platforms have their own file systems like read, write or deleting files. 

## SQLiteOpenFlag 
The enum supports these values:
- Create: Connection will automatically create the database file if it doesn't exist.
- FullMutex: Connection is opened in serializd threading mode.
- NoMutex: Connection is opened in multi-threading mode.
- Privatecache: Connection won't participate in the shared cache if its enabled.
- ReadWrite: Connection can read and write data
- SharedCache: Connection will particupate in the shared cache if enabled
- ProtectionComplete: File is encrypted and not accessible while the device is locked
- ProtectionCompleteUntilFirstUserAuthentication: The file is encrypted until after the user has booted and unlocked the device.
- ProtectionNone: Database file is not encrypted.
