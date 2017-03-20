# file transfer

## use nc(netcat)
### server:
```shell
tar -czf - <filename1> [filename2...] | nc -l <port>
```

### client
```shell
nc <host> <port> | tar -xzf - 
```

### transfer encrypted
### server:
```shell
tar -czf - <filename1> [filename2...] | openssl des -k <passwd> | nc -l <port>
```

### client
```shell
nc <host> <port> | openssl des -d -k <passwd> | tar -xzf - 
```


