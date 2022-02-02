### Latest


### 2.1.1

- Automatically trigger keyboard 'Enter/Return' action after text expansion.
- Randomly select an item from phrase list.
- Added support for German language.
- Fixes text rendering issue affecting some devices.


### Older

#### 2.0.7 


- Android 12 compatibility
- Fixes overlay UI positioning issues in Android 12

#### 2.0.6 - 8f5c29e

- Adds support for Brazilian Portuguese language 🇧🇷
- Bug fixes

#### 2.0.5 - cffbb0f

- Fixed an issue where expanded text would undo automatically.
- Intoduced a prompt to help you configure Texpand run smoothly in the background.
- Few minor improvements.

#### 2.0.4 - e7e20fc

Includes the following bug-fixes:

- “Add phrase" may not work after adding a phrase
- Phrase lists does not display item order correctly
- Crash when "sync only on wifi" preference is tapped
- Crash when Tasker user variables are used in a phrase list
- Texpand variables lose styling in some cases
- Clipboard variable hides the keyboard in Android 10 
- Space would continue to be added when "Append space" global option is disabled.
- The delete icon may not appear when editing a phrase


#### 2.0.3 - b64f984


- 📥 CSV import and export
- 🔧 Android 11 compatibility:
   - Removes the ability to launch TIA using accessibility button, because Android 11 requires it to be enabled all the time.
   - In Android 11 application management does not list installed apps, you have to manually type an app's package name to include or exclude it.
- 📋 Clipboard variable no longer require special adb permission.
- 🐞 "Expand instantly" and "Expand within words" can now work together, 'backspace to undo' is not supported when both are turned on
- ⭐️ Uses Google Play In-App review library to ask for reviews
- 👉 Removes the ability to instantly modify phrases in Google Drive to limit API usage


#### 2.0.2 - d1e48bd

- ✨ New: insert phrase from text selection, [learn more](/README?id=insert-phrases-by-replacing-text-selection)
- 🐞 Fixed: missing leading zero for single digit date
- 🐞 Fixed: auto-expansion issue, now disabling "Expand with space/punc" doesn't cause phrases to expand instantly.
- 🐞 Fixed: renamed per phrase setting "Don't require space for expansion" to "Expand instantly" if enabled a phrase will auto-expand as soon as it's typed.
- 🐞 Fixed: phrases that have "Expand within words" enabled expanded by space/punctuation

#### 2.0.1 - 6c1c5ee

- 🇪🇸 Hola! Texpand is now available in Spanish (Gracias, Nicolàs Portela)
- 👉 Removed "Phrase Preview" option
- 👉 Renamed "Don't expand by space/punctuation" to "Don't require space for expansion", now if enabled will auto-expand a shortcut and disable "Phrase Preview" for the shortcut
- 👉 Now if global setting "Expand with space/punctuation" is disabled all shortcuts will auto-expand and "Phrase Preview" will be disabled for all shortcuts
- 🐞 Fixed: undo may not work in some situations
- 🐞 Fixed: reversed predefined date formats
- ✨ Stability and performance improvements

#### 2.0.0 - 541a938 (Release)

🎊 An all new Texpand 2.0 is here 🎊

This update improves everything you love about Texpand and adds exciting new features:

- 🔄 Google Drive sync & back up
- 😍 New design with dark mode
- ⚡  Improved Tasker support
- ⚙️ Revamped settings
- 🅰  Improved Text Input Assistant 
- 🎛️ Improved per phrase settings
- ⛔ Blacklist or whitelist applications
- ⌫  Backspace to undo  
- 📚 New help pages at: https://texpandapp.com/docs
- 🔧 And more improvements
- 🐞 Fixed: a crash that occurs when a user saves 1000 or more phrases
- 🐞 Fixed: a crash when a 100 char word without space is typed.


#### Texpand 2.0.0 - 8a8641e RC3

- 🐞 Fixed a crash caused when adding/clicking Text Input Assistant quick setting tile.

- 📋 You can now simply tap an item to copy it in Text Input Assistant, if there's a focused text field underneath it will be pasted automatically https://www.texpandapp.com/docs/#/text-input-assistant?id=copypaste-phrases

- 📖 Texpand help pages are accessible from within in the app, tap "?" icon or "Help" in any screen to get help

- 🐞 Bug fixes and optimizations


##### Texpand 2.0.0 Beta 4

- 📋 Clipboard access now available in [Android 10](/text-input-assistant?id=clipboard-access-in-android-10 'target=_self')
- 👆 Added: Text Input Assistant can now be opened via [fingerprint gesture](/text-input-assistant?id=how-to-open 'target=_self')
- 🇨🇳 Texpand is now available in Chinese
- ⭐️ Implemented a much more efficient way to hide overlay UI
- 🐞 Fixed: a system wide lag that may occur when Texpand's accessibility service is enabled
- 🐞 Fixed: an issue where the text color of the search field in Text Input Assistant doesn't change with theme changes

##### Texpand 2.0.0 Beta 3

- 🐞 Fixed: couldn't reconfigure Tasker plug-in to select more user variables
- 🐞 Fixed: issue with discard dialog when creating phrase lists
- ⭐️ New: app shortcuts for creating phrase and phrase lists, settings and search
- ⭐️ New: Firebase event reporting for important user events

##### Texpand 2.0.0 Beta 2

- ⭐️ Added About screen 
- ⭐️ Minimum supported version is now Android 7.0

##### Texpand 2.0.0 Beta 1

- 🔄 Google Drive sync & back up
- 😍 New design with dark mode
- ⚡ Improved Tasker support
- ⚙️ Revamped settings
- 🎛️ Improved phrase settings
- ⛔ Blacklist or whitelist applications
- ↪️ Backspace to undo  
- 🔧 And more improvements
