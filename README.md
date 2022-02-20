This project supports PyVPR supports plate recognition of Bosnian car plates. If you want to run this project, you need to follow next instructions.

To run website on local and ngrok server, please follow next steps:
1. In PyVPR_ETF2022/django_projects_pyvpr/localdatabase terminal run:
	$ python3 manage.py superuser
2. After adding admin, run:
	$ python3 manage.py runserver
3. You need to download ngrok and make an account. After doing so, run in terminal:
	$ ngrok http -host-header=127.0.0.1 8000
4. You will get a web site URL of ngrok server.

To run local server on 127.0.0.1 5000, please follow next steps:
1. Install Flask
2. In PyVPR_ETF2022/django_projects_pyvpr/localdatabase terminal run:
	$ virtualenv .venv
	$ source .venv/bin/activate
	$ python3 app.py
3. In the same folder terminal run:
	$ chmod u+x bash_in.sh
	$ chmod u+x bash_out.sh
4. In the same folder terminal run:
	$ python3 app.py
5. Run in terminal:
	$ ngrok http -host-header=127.0.0.1 5000

To add plate number to the database, please follow next steps:
1. In PyVPR_ETF2022/projects/TSI terminal run:
	$ python3 slike.py
2. Move photo of the car you want to display in database from folder PyVPR_ETF2022/projects to folder PyVPR_ETF2022/projects/TSI
3. You will see plate number in terminal and time of uploading the photo.
4. Open the web site on http://6444-195-130-59-184.ngrok.io/catalogplates/, log in and you will see that the plate number is added to the database.

To delete plate number from the database, please follow next steps:
1. Write the plate number information to file tablica_out.txt in folder PyVPR_ETF2022/projects.
2. In PyVPR_ETF2022/projects terminal run:
	$ python3 tablice_out.py
	
This project was realized as part of Telecommunications Software Engineering course on Master's studies at University of Sarajevo, Faculty of Electrical Engineering, Department of Telecommunications in the 2021/2022. school year. Students that worked on this project are: Kemal Drnda, Merima Fehrić, Elma Kevilj, Tamara Markešić, Džana Pivač and Neira Dizdarević, alongside supervisor professor doc.dr Darijo Raca. 
