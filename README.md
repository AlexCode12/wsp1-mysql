# wsp1-mysql

## Kör igång Ubuntu
kör
  sudo service mysql restart
  sudo service apache2 restart

OM apache2 inte vill sammarbeta (BranchCache ligger på port 80)
## Följ detta steg för steg:

## Aktivitetshanteraren

## Tjänster

* Öppna Tjänster

* Sortera i bokstavsordning

* "BranchCache"

* Egenskaper

* Stoppa + Inaktivera

* Återställning

* Sedan "Ingen Åtgärd" på samtliga tre

* Verkställ

* OK

* Då funkar det!

## MYSQL

**setup**
Kör
	sudo mysql -u root
	
För att få till localhost/~användarnamn
Gå till 	
	etc/apache2

Kör:

	sudo a2enmod userdir
Och


	sudo service apache2 restart
	
	
för nya användare:
	
	grant all privileges on *.* to 'username'@'localhost' identified by 'password';


För att ändra i PHP:n (kommentera bort):

Gå till och kör:

	
	cd mods-aviable/
	sudo nano php7.2.conf
	sudo service apache2 restart
