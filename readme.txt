1) Place data.db somewhere and replace the location in this

	'char *database = "/mnt/HDD/data.db";'

line of void InitializeDatabase() function of Database.c file of RentmanagerService. Compile and run.

2) JavaFX Controls module need JavaFX Services reference
3) JavaFX RentManager module need both Controls and Services reference
4) reference JavaFX library and in vm args give it --add-modules javafx.controls
5) run (I'm on IntelliJ IDEA)
