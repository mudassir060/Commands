### install the stacked_cli package on your machine:
    dart pub global activate stacked_cli
### Update CLI
    stacked update

### Creating a new Stacked App
    stacked create app my_app

### Creating a new view
    stacked create view login

### Creating a new service
    stacked create service stripe

### Creating a new Bottom Sheet
    stacked create bottom_sheet alert

### Creating a new Dialog
    stacked create dialog error

### Creating a new widget
    stacked create widget users_list

### Generate Code
When you've changed something manually, or added a new model
    flutter pub run build_runner build --delete-conflicting-outputs