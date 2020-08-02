## Mission Lab Utilities
This is the very start of a collection of simple Automator programs to help with simple, repeatable steps in a Mission lab/on set workflow.

It is based around the idea of storing some 'variables' in simple text files in a `$HOME/lab_config folder`.


Here is a brief summary of each applet:

- ### Set MEDIARAID Directory
This should be run once at the start of a project. It will ask you to point to your projects MEDIARAID directory, the app will then store this folder path in the file: `$HOME/lab_config/mediaraid_project_directory.txt` for use by other applets later.

- ### Set Todays Shootday
This should be run at the start of each shoot day. It will ask for a text string input of the current shoot days folder name, such as YYYYMMDD_SHOOTDAY_XXX. This string will then be stored in `$HOME/lab_config/current_shootday.txt` for use by other applets later.

- ### Move Todays Docs
This requires the previous two steps have been done so you have a MEDIARAID directory and a current shootday value stored. It will move files within `$HOME/Desktop/_TODAY` to your working MEDIARAID shoot day directory.
