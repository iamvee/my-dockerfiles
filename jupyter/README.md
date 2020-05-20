
## build


```bash
docker build -t jupyter:latest .    
```

## run

```bash
docker run -p 8080:8080 -it -v $PWD/data:/root jupyter:latest
```