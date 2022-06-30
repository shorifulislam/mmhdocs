# Publishing to IIS

Publishing ASP.NET Zero Core MVC project is no different to any other ASP.NET Core Applications.

## Publishing Web Site

- Right click `\*.Web.Mvc` project and click **Publish**.
- Click **Start** and select **Folder** tab and choose the URL that you want to publish.

<img src="images/iis-core-publish-select-folder-and-publish.png">

- Create a folder on the server where **IIS** is located. (for example: `C:\inetpub\wwwroot\mywebsite`).
- Copy extracted files to server. (from `\*.Web.Mvc/bin/Release/netcoreapp2.1/publish/` to `C:\inetpub\wwwroot\mywebsite`).
- Change `appsettings.production.json` configurations with your own settings.

## Create IIS Web Site

- Right click **Sites** and click **Add Website**.

<img src="images/iis-core-publish-add-website-to-iis.png">

- **mywebsite** application pool will be created automatically. Click **Application Pools**, double click **mywebsite** application pool and change its configuration.

<img src="images/iis-core-publish-configure-app-pool.png">


The project contains a `web.config` file, its contents may be changed during development, please check the` web.config` file after publishing, especially the `ASPNETCORE_ENVIRONMENT` setting.

For instructions on how to install the ASP.NET Core Module, see [Install the .NET Core Hosting Bundle](https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/index?view=aspnetcore-2.1#install-the-net-core-hosting-bundle).

For more information see [Host ASP.NET Core on Windows with IIS](https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/index?view=aspnetcore-2.1) document

