# How to run this demo in Docker?
## To run this demo, run the command below:
```
git clone https://github.com/saga-pattern-demo/how-to-run.git
```
## Please ensure that Docker is running and execute this command.
```
docker-compose up -d
```
</br>

# How to test?
## Let's review my data before the test.
user balance
```
userID 1: 100$
userID 2: 100$
userID 3: 200$
```
product price
```
productID 1: 20$
productID 2: 30$
productID 3: 50$
```
stock quantity
```
productID 1: 5
productID 2: 5
productID 3: 3
```

## Send a post request to create a new order
```
curl -d "{\"userID\":1,\"productID\":3}" -H "Content-Type: application/json" http://localhost:8091/api/v1/orders
```
## Send a get request to get all orders
```
curl -v http://localhost:8091/api/v1/orders
```
