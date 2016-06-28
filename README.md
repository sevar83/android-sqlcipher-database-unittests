# android-sqlcipher-database-unittests

**Some Unit tests for https://github.com/sqlcipher/android-database-sqlcipher ported from AOSP.**

- Has a Gradle dependency on SQLCipher 3.5.1
- Some tests are commented out because they cannot be compiled with the minSDK=7 requirement of SQLCipher. (stuff like CancelationSignal introduced in API14+).
- Adapted to the lasted Android testing library.
- Tests Android N support (targetSDK=24).

**Usage**

Open in Android Studio 2.2+ (or other version able to build with Android N)
In Project Explorer expand and right-click on "app > java > net.sqlcipher.unittests (androidTest)"
Click "Run Tests in net.sqlcipher.unittests"

*Note*
Some tests are normal to fail as SQLCipher works in a different than the platform SQLite API.
