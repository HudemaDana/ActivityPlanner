# Activity Planner
The application:
1. Manage persons and activities. The user can add, remove, update, and list both persons and activities.
2. Add/remove activities. Each activity can be performed together with one or several other persons, who are already in the user’s planner.
3. Search for persons or activities. The search is case-insensitive, partial string matching, returning all matching items.
4. Create statistics:
    a. List the activities for a given date, in the order of their start time.
    b. Busiest days. This will provide the list of upcoming dates with activities, sorted in ascending order of the free time in that day (all intervals with no activities).
    c.List all upcoming activities to which a given person will participate.
5. Unlimited undo/redo functionality.
6. Uses two additional repository sets: text files and binary files.
7. The decision of which repositories are employed, as well as the location of the repository input files are made in the program’s `settings.properties` file.
   Exemple:
    `settings.properties` for loading from memory (input files are not required):
    ```
    repository = inmemory
    person = “”
    activity = “”
    ```
