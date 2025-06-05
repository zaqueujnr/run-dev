Repo para subir o sistema com docker em modo desenvolvimento.

## 🚀 Para rodar o projeto em desenvovimento com Docker

- git clone https://github.com/zaqueujnr/front-end (-> develop) 
- git clone https://github.com/zaqueujnr/back-end (-> develop) 
- git clone https://github.com/zaqueujnr/run-dev (-> develop) 
- cd run-dev/
  
- set ../back-end/.env.db ../back-end/.env.dev 

- .env.db.example

  POSTGRES_USER=postgres |
  POSTGRES_PASSWORD=password 

- .env.dev.example
  
  PORT=3000 |
  DATABASE_URL=postgres://postgres:password@db-dev:5432/mydb |
  SKIP_DOTENV=false 

- docker-compose -f docker-compose.dev.yml up --build  

