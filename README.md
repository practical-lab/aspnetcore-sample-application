# aspnetcore-sample-application

![Docker Image CI](https://github.com/practical-lab/aspnetcore-sample-application/workflows/Docker%20Image%20CI/badge.svg)

## dotnet cli

### Create project

```bash
dotnet new web -o aspnetapp
```

### Run

```bash
dotnet run -c Debug
```

### Create sln

```bash
dotnet new sln
```

### Add sln

```bash
dotnet sln add aspnetapp/aspnetapp.csproj
```

## Docker

### Build image

```bash
docker build -t docker.pkg.github.com/practical-lab/aspnetcore-sample-application/web-application:0.1 .
```

### Run container

```bash
docker run --rm -it -p 8000:80 docker.pkg.github.com/practical-lab/aspnetcore-sample-application/web-application:0.1
```

### Push image

```bash
docker push docker.pkg.github.com/practical-lab/aspnetcore-sample-application/web-application:0.1
```
