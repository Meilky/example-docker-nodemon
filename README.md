#Example

Build the app:
```bash
docker build . -t <build-type>/web-app --target=<build-type>


docker build . -t dev/web-app --target=dev
```

Run the app:
```bash
docker run -p <port>:3000 -v "$PWD/src:/usr/app/src" <build-type>/web-app

docker run -p 3000:3000 -v "$PWD/src:/usr/app/src" dev/web-app
```
