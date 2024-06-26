# Football_Manager_Program2
This Java application serves as a football management system, enabling the creation, modification, deletion, and management of clubs, teams, players, and trainers. The system is designed to handle the complexities of football management including team assignments, transfers, and data persistence using a MySQL database.

## Features

- Manage clubs, teams, players, and trainers
- Add and remove entities with ease
- Assign players and trainers to teams
- Transfer players and trainers between teams or to a free pool
- Persistent data storage in a MySQL database
- Interactive command-line interface for easy navigation and management

## Usage

Upon launching the Football Manager application, you will encounter the main menu. The application is designed to be interacted with via a command-line interface where you can manage football clubs, teams, players, and trainers. Below is a breakdown of the main menu and the operations you can perform:

### Main Menu
When you start the application, the main menu displays the following options:
```
*** Welcome to Football Manager ***
[1] Club
[2] Team
[3] Player
[4] Trainer
[5] Manual
[0] Exit program
Enter the index of your choice:
```
Each option leads to a specific submenu where you can perform related operations. To navigate, you enter the number associated with your choice.

### Club Management
From the club menu, you can add, delete, show, or edit clubs:
```
*** Club Menu ***
[1] Add Club
[2] Delete Club
[3] Show Club
[4] Edit Club
[0] Back to Main Menu
Enter the index of your choice:
```
- **Add Club**: Enter the name and establishment year, and the club will be registered in the system.
- **Delete Club**: Remove an existing club from the system.
- **Show Club**: Display details of all clubs.
- **Edit Club**: Modify details of an existing club.

### Team Management
This menu allows you to manage teams within a club:
```
*** Team Menu ***
[1] Add Team
[2] Delete Team
[3] Show Team
[4] Edit Team
[0] Back to Main Menu
Enter the index of your choice:
```
- **Add Team**: Create a new team under a specific club.
- **Delete Team**: Remove a team from a club.
- **Show Team**: List all teams under a specific club.
- **Edit Team**: Update details of a specific team.

### Player Management
Players can be managed through this menu:
```
*** Player Menu ***
[1] Add Player
[2] Delete Player
[3] Show Player
[4] Edit Player
[5] Transfer Players
[0] Back to Main Menu
Enter the index of your choice:
```
- **Add Player**: Register a new player as free or to a team.
- **Delete Player**: Remove a player from the system.
- **Show Player**: Display all players or only free players.
- **Edit Player**: Change details of an existing player.
- **Transfer Players**: Move a player between teams or to the free pool.

### Trainer Management
Similar to players, trainers can be added, removed, shown, or edited:
```
*** Trainer Menu ***
[1] Add Trainer
[2] Delete Trainer
[3] Show Trainer
[4] Edit Trainer
[5] Transfer Trainers
[0] Back to Main Menu
Enter the index of your choice:
```
- **Add Trainer**: Enlist a new trainer either to a team or as free.
- **Delete Trainer**: Expunge a trainer from the database.
- **Show Trainer**: View details of all trainers or only those unassigned.
- **Edit Trainer**: Modify the particulars of a trainer.
- **Transfer Trainers**: Reassign trainers among teams or set as free.

### Manuals
The application also provides a manual for guidance:
```
*** Manual Menu ***
[1] English Manual
[2] Deutsch Manual
[0] Back to Main Menu
Enter the index of your choice:
```
Select the language of the manual you wish to view.

### Exiting the Program
To exit the program, select `0` from the main menu. Make sure to save any changes or finish your operations before exiting to avoid loss of data.

## Development

The project is structured into multiple packages to organize the codebase effectively:
- `manager.club` for club-related operations
- `manager.player` for player management
- `manager.team` for team management
- `manager.trainer` for trainer operations
- `manager.database` for database interactions
- `manager.menu` for user interface interactions
- `manager.function` for universal operations
