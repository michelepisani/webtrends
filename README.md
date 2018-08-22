# webtrends
Webtrends Community Connector for Google Data Studio

*This is not an official Google product*

![webtrends data studio community connector](https://user-images.githubusercontent.com/8077996/44444251-3e374d80-a5dc-11e8-8714-be77c7af53c0.png)

This [Data Studio](https://datastudio.google.com) [Community
Connector](https://developers.google.com/datastudio/connector) allows users to access all of their [Webtrends](https://www.webtrends.com/) data in Google Data Studio. This Community Connector uses the **Webtrends API**.

## Try the Community Connector in Data Studio

You can try out the managed deployment of the latest code: [Webtrends Community Connector](https://datastudio.google.com/datasources/create?connectorId=AKfycbzSrtEqnF5eyipfxPs9jmfYpXHZXGZoW7DFiYLhYTgo5GbQsuXjNeU0OKoxTrN4SHT7TA)
This community connector require the authentication credentials to login to your Webtrends account.

## Deploy the Community Connector yourself

1. Visit [Google Apps Script](https://script.google.com/) and create a new project.
2. You should see a shell project with a blank `myFunction` function in the `Code.gs` file. Delete the `myFunction` function and copy over the contents of the `main.js` file from the repository.
3. If the repository has any other `.js` or `.gs` file, you will need to create those files in Apps Scripts environment(**File > New > Script File**) and copy over the content.
4. In the Apps Script development environment, select **View > Show manifest file**. This will create a new `appsscript.json` manifest file. Remove all content from this manifest file and replace it with the content of the `appsscript.json` file in the repository.
5. To use the Community Connector in Data Studio, follow the [guide on Community Connector Developer site](https://developers.google.com/datastudio/connector/use).

##
For information on how to use the connector and support requests refer to the dedicated page on the developer's website: [appsscript.it](http://www.appsscript.it/articoli/data-studio-connector-webtrends-connettore-personalizzato/).

## Examples and use cases covered in the connector

- **USER_PASS authentication**  
  This community connector require the authentication credentials to login to your Webtrends account.
  Once the login credentials have been approved, it will be enough to provide the ID of your Webtrends Account and the ID of the Report you want to query before connecting.
- **Dynamic Schema**  
  Example of automatic generation of a dynamic schema based on the response of the requested Report ID, [getSchema()](https://developers.google.com/datastudio/connector/reference#getschema).
