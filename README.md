### Installing necessary packages:  
* `pip install fastapi`
* `pip install "uvicorn[standard]"`  
* `pip install sqlalchemy`  
* `pip install pymysql`
* `pip install pytest`
* `pip install pytest-mock`
* `pip install httpx`
* `pip install cryptography`

Or install all dependencies at once:

`pip install -r requirements.txt`

### Configure MySQL:
1. Start your local MySQL server.
2. Create the assignment database if it does not already exist:

`CREATE DATABASE sandwich_maker_api;`

3. Update `api/dependencies/config.py` if your MySQL username, password, host, port, or database name are different.

### Run the server:
`uvicorn api.main:app --reload`

### Test API by built-in docs:
[http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

### Available CRUD resources:
* `/orders/`
* `/sandwiches/`
* `/resources/`
* `/recipes/`
* `/order-details/`
