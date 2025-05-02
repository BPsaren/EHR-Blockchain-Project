# EHR-Blockchain-Project

This project integrates health records with blockchain technology to secure patient data effectively. Utilizing Ethereum-based smart contracts and decentralized off-chain storage via the Inter Planetary File System (IPFS), the framework ensures data protection and scalability. Blockchain guarantees that only authorized personnel can update, delete, or exchange patient records, enhancing security and transparency. MetaMask is used for blockchain interactions, with Python powering the backend. HTML structures the content, and CSS adds styling. The framework employs strong symmetric encryption, blockchain, and IPFS to safeguard Electronic Health Records (EHR), delivering a robust and secure solution for the healthcare sector.

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher)
- [Python](https://www.python.org/downloads/) (v3.8 or higher)
- [Ganache](https://trufflesuite.com/ganache/) (local blockchain for development)



## Step 1 (Run Locally)

I. Fork and Clone the Repository

```bash
  git clone git@github.com:BPsaren/EHR-Blockchain-Project.git
```

II. Go to the project directory

```bash
  cd EHR-Blockchain-Project
```

III. Install Frontend Dependencies

```bash
  cd client
  npm install
```


IV. Install Python dependencies(Backend)

```bash
  pip install -r requirements.txt
```
    

V. Database Setup with SQLite(Create and apply migrations)

```bash
python manage.py makemigrations
python manage.py migrate
```


VI. Create a Superuser (Admin) . Follow prompts to create an admin account.

```bash
python manage.py createsuperuser
```

VII. Start the Development Server
```bash
python manage.py runserver
```
By default, this will start the server at: http://127.0.0.1:8000/


###  Verify It's Working or not
Visit http://127.0.0.1:8000/admin to access Django admin

Visit your API endpoints (e.g., http://127.0.0.1:8000/api/patients/)

## Step 2 

I. Add truffule-config in Ganache

![App Screenshot](https://github.com/BPsaren/EHR-Blockchain-Project/blob/4923748c1dacdb2aad8e7dc5cc352e91360f6b89/ganache_truffle.PNG)

II. Starts development server (frontend)

```bash
  yarn start
```

III. Deploys smart contracts to the blockchain (compiles + runs migrations)

```bash
  truffle migrate
```

## Congratualiton you successfully deploy the server

![App Screenshot](https://github.com/BPsaren/EHR-Blockchain-Project/blob/c65c90b9fa1094f5382f92b4582f8b5f4026a100/UI.PNG)
