deploy with ```vagrant up```

query a function from within the VM through:
```
curl -H "Host: [FUNCTION].default.localhost" -X POST -d "test" http://127.0.0.1:[PORT]
```
where [PORT] is the port number you get with
```sudo -E kubectl --namespace kourier-system get service kourier```
