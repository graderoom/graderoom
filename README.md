# Graderoom
Grade visualization with automatic web scraping from Powerschool for students.

## Setup  
- install Python 3.13.0
- install Node.js 22.12.0
- install redis-server
- install mongodb
- create a `.env` file with the keys in `.env.example`

### From project root
- `pip install -r requirements.txt`
- `npm i`

## Starting the server
### Stable
- Run `redis-server &` in terminal
- Set the port in `.env` to `5996`
- From project root, `node server/graderoom.js`

### Beta
- Run `redis-server --port 6381 &` in terminal
- Set the port in `.env` to `5998`
- From project root, `node server/graderoom.js`

## Accessing the website
- Navigate to `127.0.0.1:[port]` in your browser, where `port` is `5996` for stable and `5998` for beta
- A default account will be created with the following credentials:
  - Username: `admin`
  - Password: `Pa5sw0rd`
