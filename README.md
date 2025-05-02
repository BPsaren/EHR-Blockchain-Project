# EHR-Blockchain-Project

Introduction
An Electronic Health Record (EHR) is a digital version of a patient’s medical file that compiles a wide spectrum of healthcare data. It includes vital elements such as demographic details, clinical issues, medication history, physician assessments, vital signs, past medical records, immunizations, lab results, radiology reports, personal identifiers,progress updates, and billing records.

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher)
- [Python](https://www.python.org/downloads/) (v3.8 or higher)
- [Ganache](https://trufflesuite.com/ganache/) (local blockchain for development)



## Run Locally

1.Fork and Clone the Repository

```bash
  git clone git@github.com:BPsaren/EHR-Blockchain-Project.git
```

2.Go to the project directory

```bash
  cd EHR-Blockchain-Project
```

3.Install Frontend Dependencies

```bash
  cd client
  npm install
```





4.Install Python dependencies(Backend)

```bash
  pip install -r requirements.txt
```
    

4.Database Setup with SQLite(Create and apply migrations)

```bash
python manage.py makemigrations
python manage.py migrate
```


5.Create a Superuser (Admin) . Follow prompts to create an admin account.

```bash
python manage.py createsuperuser
```

6.Start the Development Server
```bash
python manage.py runserver
```
By default, this will start the server at: http://127.0.0.1:8000/


### 6. Verify It's Working or not
Visit http://127.0.0.1:8000/admin to access Django admin

Visit your API endpoints (e.g., http://127.0.0.1:8000/api/patients/)

<a href="https://ibb.co/XxDMnxVR"><img src="https://i.ibb.co/XxDMnxVR/tabular.png" alt="tabular" border="0"></a>
