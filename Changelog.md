## Updated main.py, requirements.txt, version 06/01/2024
- Version bump (24.06)
- Updated "requests" version requirent to `2.32.0` because of CVE-2024-35195
- Fixed some formatting inconsistancies (blank spaces, single quotes, command format)
- Updated code comments
- Added Play Store crashing fix by re-installing after initial Gapps install
- Replaced `os.system` & `os.popen` commands with `subprocess` equivalents since they are deprecated
- Update tool now uses Python's `os.chmod` instead of running chmod as a shell command
- Appinstaller function can now accept individual applications instead of installing all apps in a folder
- Simplified "customlauncher" function by only calling appinstaller script once
- Custom DNS check now uses try/except instead of Bash/Posix operators inside ADB shell
- xdg-open/open -e commands now use try/except instead of Bash/Posix operators
- Enabled/disabled packages on the UI are now generated by enabled & disabled list (might be easier to update lists on the fly)
