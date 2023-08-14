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
## Send a post request to create a new order
```
curl -d "{\"userID\":1,\"productID\":3}" -H "Content-Type: application/json" http://localhost:8091/api/v1/orders
```
## Send a get request to get all orders
```
curl -v http://localhost:8091/api/v1/orders
```
