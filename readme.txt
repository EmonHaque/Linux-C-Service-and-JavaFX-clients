Experimental, on Void Linux, not sure how far will I go with JavaFX!

1) Place data.db somewhere and replace the location in this

	'char *database = "/mnt/HDD/data.db";'

line of void InitializeDatabase() function of Database.c file of RentmanagerService. Compile and run.

2) place Logins.db somewhere and replace the location in this

	char* database = "/home/emon/Downloads/Logins.db";
	
line of void InitializeDatabase() function of Database.c file of LoginService. Compile and run.

3) JavaFX Controls module needs JavaFX Services reference
4) JavaFX RentManager module needs both Controls and Services reference
5) reference JavaFX library and in vm args give it --add-modules javafx.controls
6) run (I'm on IntelliJ IDEA)
7) to turn off LoginWindow, in public void start(Stage stage) of Controls/ClientApp, set var debug = true;
