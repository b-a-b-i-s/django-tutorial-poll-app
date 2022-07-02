# django-tutorial-poll-app

## Οδηγίες Εγκατάστασης Backend

### Project Download

```bash
git clone https://gitlab.com/sfhmmy/django-tutorial-poll-app.git
```

### Είσοδος στον φάκελο του project

```bash
cd mysite
```

### Εγκατάσταση Python

Windows:
<https://www.python.org/downloads/windows/>

Linux:

```bash
sudo apt install python3
python3 --version
expected output: Python 3.x.x
```

### Δημιουργία Virtual Environment στην Python

Windows:

```powershell
python -m venv .venv_django_tutorial
.venv_django_tutorial\Scripts\activate
```

Linux και OS X:

```bash
python3 -m venv .venv_django_tutorial
source .venv_django_tutorial/bin/activate
```

### Εγκατάσταση Απαιτήσεων (μέσα στο Virtual Environment)

Αν τρέχετε Linux πρέπει πρώτα να τρέξετε την ακόλουθη εντολή για να μπορέσει να εγκατασταθεί αργότερα το psycopg2:

```bash
sudo apt-get install python3-dev default-libmysqlclient-dev build-essential libpq-dev
```

Στη συνέχεια στα Linux ή στα Windows τρέξτε:

```bash
pip install -r requirements.txt
```

Το app polls μπορείτε να το βρείτε στο [github.com/b-a-b-i-s/django-polls-babis](https://github.com/b-a-b-i-s/django-polls-babis)

### Environmental variables

Φτιάξτε ένα αχρείο .env με πρότυπο το αρχείο .env.sample όπου ορίζετε τις μεταβλητές που χρειάζονται.

### Δημιουργία Μοντέλων

Windows:

```powershell
python manage.py migrate
```

Linux:

```bash
python3 manage.py migrate
```

### Σελίδα

Την σελίδα μπορείτε να τη βρείτε εδώ: <https://django-tutorial-poll-app.herokuapp.com/polls/>
