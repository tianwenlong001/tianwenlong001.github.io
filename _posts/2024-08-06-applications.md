---
layout: post
title: Cryptography
subtitle: by twl
gh-repo: tianwenlong001/tianwenlong001.github.io
gh-badge: [star, fork, follow]
tags: [learning]
comments: true
---


- [ASP.NET](#aspnet)
- [UML](#uml)


##### ASP.NET

https://www.jetbrains.com/dotnet/guide/tutorials/aspnet-basics/

https://github.com/LiangLliu/LanzhouBeefNoodles

https://www.imooc.com/video/20421



https://learn.microsoft.com/en-us/aspnet/core/?view=aspnetcore-7.0

https://learn.microsoft.com/en-us/dotnet/core/docker/build-container?tabs=windows&pivots=dotnet-7-0

https://github.com/mahedee/articles/blob/master/microservices/Dockerize_Both_MySQL_And_ASP_NET_Core_Web_App_In_Windows_Container.md

`dotnet new mvc -n myproject`

`dotnet build *.csproj  -c Release -o /app/build`

`dotnet publish *.csproj -c Release -o /app/publish`

```dockerfile
FROM mcr.microsoft.com/dotnet/sdk:7.0 AS build-env 
WORKDIR /App  
# Copy everything 
COPY . ./ 
# Restore as distinct layers 
RUN dotnet restore 
# Build and publish a release 
RUN dotnet publish -c Release -o out  
# Build runtime image 
FROM mcr.microsoft.com/dotnet/aspnet:7.0 
WORKDIR /App 
COPY --from=build-env /App/out . 
ENTRYPOINT ["dotnet", "DotNet.Docker.dll"]
```

`docker build -t myproject .`

docker run -d -p 8080:80 -it  --rm myproject

docker exec -it container_name /bin/bash 

.NET 6 + EF Core + MySQL + Docker + Identity +MVC 学习笔记 

https://www.cnblogs.com/jacky-zhang/p/16449004.html

appsetings.json

"ConnectionStrings": {

 "DefaultConnection": "Server=localhost;port=3306;Database=mydatabase;User Id=root;Password=root;",

 "IDContextConnection": "Server=127.0.0.1;Port=3306;Database=mydatabase;Uid=root;Pwd=root;"

},

EF commands:
Add-Migration init -context IDContext
update-database -Context IDContext


##### UML 
PlantUML 