# blazor-webassembly-aadb2c-hosted-net8
 
## 概要

ASP.NET Core でホストされた Blazor WebAssembly で、Azure Active Directory B2C が統合されている .NET 8 のテンプレートです。

## 事前準備

### `appsettings.json` の修正
`\Client\wwwroot\appsettings.json` と `\Server\appsettings.json` に実際の値を埋めます。  
何の値を入れたらいいのかわからない場合は、以下の記事も合わせて参照してください。  
https://blazor-master.com/azure-active-directory-b2c/

`DefaultAccessTokenScope` には、`https://{テナントのドメイン名}/{呼び出すサーバー API のアプリ ID URI}/{スコープ名}` を入れます。  
（例）`https://hoge.onmicrosoft.com/6518a3e3-b571-4402-bddd-e89f29bafa3e/API.Access`
