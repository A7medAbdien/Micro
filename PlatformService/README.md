1. create project
```sh
dotnet new webapi -n PlatformService
```

2. delete unneeded form template

3. install dependencies
```sh
dotnet add package AutoMapper.Extensions.Microsoft.DependencyInjection

dotnet add package Microsoft.EntityFrameworkCore

dotnet add package Microsoft.EntityFrameworkCore.Design   

dotnet add package Microsoft.EntityFrameworkCore.InMemory 

dotnet add package Microsoft.EntityFrameworkCore.SqlServer

```

4. create platform model

5. Data layer

6. Adding startup files
there is no startup file in sdk 6, so i followed [this](https://www.talkingdotnet.com/clean-way-to-add-startup-class-in-asp-net-core-6-project/) and understood that form [this](https://www.reddit.com/r/csharp/comments/t4qmq4/aspnet_core_6_how_to_deal_with_the_missing/)

worth mentioning that i tried to move to sdk 5.0.3 but there were an error in installing the dependencies step because the compatibility of `Microsoft.EntityFrameworkCore`