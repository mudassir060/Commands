### install the stacked_cli package on your machine:
    dart pub global activate stacked_cli
### Update CLI
    stacked update

### Creating a new Stacked App
    stacked create app my_app

### Creating a new view
    stacked create view login
This command creates all the scaffolding to add a new View into the project:

1-Creates a new folder with the View name in lib/ui/views/
2-Creates the new View and ViewModel files in lib/ui/views/view_name/
3-Creates the ViewModel tests file in the test/viewmodel_tests/ folder
4-Adds the route to the lib/app/app.dart file

### Creating a new service
    stacked create service stripe
This command creates all the scaffolding to add a new Service into the project:

1-Creates a new Service file in lib/services/
2-Creates the unit tests file in test/services/
3-Registers the Service with your StackedApp

### Creating a new Bottom Sheet
    stacked create bottom_sheet alert
This command creates all the scaffolding to add a new BottomSheet into the project:

1-Creates a new folder with the Sheet name in lib/ui/bottom_sheets/
2-Creates a new Sheet file in lib/ui/bottom_sheets/sheet_name/
3-Registers the BottomSheet with your StackedApp
### Creating a new Dialog
    stacked create dialog error
This command creates all the scaffolding to add a new Dialog into the project:

1-Creates a new folder with the Dialog name in lib/ui/dialogs/
2-Creates a new Dialog file in lib/ui/dialogs/dialog_name/
3-Registers the Dialog with your StackedApp
### Creating a new widget
    stacked create widget users_list

### Generate Code
    flutter pub run build_runner build --delete-conflicting-outputs
When you've changed something manually, or added a new model


### Stacked commands:
  compile    Uses the /templates folder and creates the appropriate template code required for the scaffolding.
  create     Provides access to the different creation tools we have for stacked.
  delete     Provides access to the different deletion tools we have for stacked.
  generate   Generates the code for the stacked application if any changes were made.
  update     Updates stacked_cli to latest version.

  ### create subcommands:
  app            Creates a Stacked application with all the basics setup.
  bottom_sheet   Creates a bottom sheet with all associated files and makes necessary code changes for adding a bottom sheet.
  dialog         Creates a dialog with all associated files and makes necessary code changes for adding a dialog.
  service        Creates a service with all associated files and makes necessary code changes to include that service.
  view           Creates a view with all associated files and makes necessary code changes for adding a view.
  widget         Creates a widget with their model file.

### delete subcommands:
  service   Deletes a service with all associated files and makes necessary code changes for deleting a service.
  view      Deletes a view with all associated files and makes necessary code changes for deleting a view.