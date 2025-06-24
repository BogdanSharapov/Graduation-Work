Шарапов Богдан Косимович
г.Казань ул.Железнодорожников, д.19, кв.32; +7(903)-804-65-39
Выпускная квалификационная работа на тему: "Разработка платформы для агентства недвижимости"
Руководитель: Титовцев Антон Сергеевич, профессор каф. ИСУИР, д.т.н., доцент.
Казанский национальный исследовательский технологический университет (ФГБОУ ВО «КНИТУ»). Институт управления, автоматизации и информационных технологий (ИУАИТ). Специальность: 02.03.03 Математическое обеспечение и администрирование информационных систем.

Информация о продукте:
Веб-платформа для агентства недвижимости "Здесь и Сейчас". Разработана на платформе ASP.NET Core MVC. С использованием PostgreSQL и LiteDB.
Для успешного развёртывания продукта необходимо установить Microsoft Visual Studio и установить следующие пакеты в NuGet менеджере:
<ItemGroup>
  <PackageReference Include="Microsoft.AspNetCore.Identity.EntityFrameworkCore" Version="8.0.11" />
  <PackageReference Include="Microsoft.AspNetCore.Identity.UI" Version="8.0.11" />
  <PackageReference Include="Microsoft.EntityFrameworkCore" Version="9.0.4" />
  <PackageReference Include="Microsoft.EntityFrameworkCore.Design" Version="9.0.4">
  </PackageReference>
  <PackageReference Include="Microsoft.EntityFrameworkCore.Sqlite" Version="8.0.11" />
  <PackageReference Include="Microsoft.EntityFrameworkCore.SqlServer" Version="9.0.4" />
  <PackageReference Include="Microsoft.EntityFrameworkCore.Tools" Version="9.0.4">
  </PackageReference>
  <PackageReference Include="Microsoft.Extensions.Configuration" Version="9.0.5" />
  <PackageReference Include="Microsoft.Extensions.Configuration.Abstractions" Version="9.0.5" />
  <PackageReference Include="Microsoft.Extensions.Configuration.Json" Version="9.0.5" />
  <PackageReference Include="Microsoft.VisualStudio.Web.CodeGeneration.Design" Version="8.0.7" />
  <PackageReference Include="Npgsql.EntityFrameworkCore.PostgreSQL" Version="9.0.4" />
  <PackageReference Include="Swashbuckle.AspNetCore.SwaggerGen" Version="8.1.1" />
  <PackageReference Include="Swashbuckle.AspNetCore.SwaggerUI" Version="8.1.1" />
</ItemGroup>
Так же необходимо добавить в зависимости сервис ImageStorage:
 <ItemGroup>
   <ProjectReference Include="..\ImageStorage\ImageStorage.csproj" />
 </ItemGroup>
В БД развернуть бэкапы для PostgreSQL и LiteDB - приложенные в архиве.
