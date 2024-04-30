# Llama 2 service

## Building and running

```
./mvnw spring-boot:run
```

## Access the endpoint

To get a response to the default request of "Tell me a joke"

```shell 
curl http://localhost:8080/llama2/generate
```

A sample response is 

```text
Sure, here's a classic one for you:

Why don't scientists trust atoms?

Because they make up everything!
```

Now using the `message` request parameter
```shell
curl --get  --data-urlencode 'message=Tell me a joke about a cow.' http://localhost:8080/llama2/generate 
```

A sample response is

```text
Why did the cow go to space?

Because it wanted to see the mooooon!
```

Alternatively use the `httpie` clinet
```shell
http 
```
