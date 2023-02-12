Rent Manager / RentManagerService
----------------------------------------------
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
==============================================

WPF version of RentManager in Windows 10 uses 2-5% CPU and 50-60% GPU. In Linux, this JavaFX version uses 100% of one or more CPU cores and 100 % of GPU when animations are in action. Just keep moving mouse over any refresh button and look at the CPU/GPU usage in Linux. In Windows 10 this JavaFX version uses 5-20% CPU and 60-80% GPU, hmm.
---------------------------------------------------

Bills / BillService

1) database sql is in WPF Bills repo
2) change char *database = "/mnt/HDD/bills.db" in void InitializeDatabase() function of Database.c;
3) you need an image folder for images you save after paying Desco, WASA, Titas Gas and BTCL bills via Nagad mobile postal Service. Change static char *imageDirectory = "/mnt/HDD/images/" of Database.c;
4) it's a dependency on tess4j (requires tesseract-ocr).
5) Bills-JNA doesn't require tess4j (needs tesseract-ocr and opencv4)
