## tuscola_backend
Project Work L31 Informatica per le aziende digitali Backend

Queste instruzioni sono preparate per installare un piccolo ambiente di sviluppo su di un sistema operativo Windows

## DIAGRAMMA ER 

Nel repository è presente il Diagramma ER del Database docs/ERDiagram.pdf

Per l'installazione del Backend si può procedere con i seguenti passi:

## APACHE E MYSQL

Installare Xampp che comprende sia il web server apache che il database relazionale MySql

[XAMPP](https://www.apachefriends.org/it/download.html)

## PYTHON

Scaricare ed installare la corretta versione di Python dal sito :

[Python](https://www.python.org/downloads/)

Installare le seguenti dipendenza python direttamente dal prompt dei comandi

# Flask
L’installazione avviene attraverso il comando Python da prompt dei comandi:

```bash
pip install Flask
```

# Flask-CORS
L’installazione avviene attraverso il comando Python da prompt dei comandi:

```bash
pip install -U flask-cors
```

# MySQL Connector
L’installazione avviene attraverso il comando Python da prompt dei comandi:

```bash
pip install mysqlconnector

pip install mysql-connector-python
```

# Bcrypt
L’installazione avviene attraverso il comando Python da prompt dei comandi:

```bash
pip install bcrypt
```

# Datetime
L’installazione avviene attraverso il comando Python da prompt dei comandi:

```bash
pip install datetime
```

## DATABASE

Importare, utilizzando la console di xampp http://localhost/phpmyadmin/ il dump del database docs/tuscola_mngt.sql

Impostare, nelle prime righe (17-21) del file tucola_api.py il corretto utente di db DB_USER, DB_PASSWORD :

```
        connection = mysql.connector.connect(
            host='localhost',
            database='tuscola_mngt',
            user='DB_USER',
            password='DB_PASSWORD'
```

## TEST

Avviare Xampp e lanciare il database MySql dal tasto MySql -> Start

Posizionare il contenuto del repository (cartella python) in una directory del disco C: ad esempio C:\tuscola_backend

lanciare l'app tuscola_api con il seguente comando:

```bash
python tuscola_api.py
```

## DOCUMENTAZIONE

[Diagramma ER](https://github.com/Paoletto73/tuscola_backend/blob/main/docs/ERDiagram.pdf)

[Dump Database](https://github.com/Paoletto73/tuscola_backend/blob/main/docs/tuscola_mngt.sql)


