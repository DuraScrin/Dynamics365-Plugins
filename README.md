# Dynamics365-Plugins

Pre-pare Dynamics 365 enviroment<br/>
  Cteate a publisher in Dynamics
    Settings -> Customizations -> Publishers
  Create sollution in Dynamics
    Settings > Solutions -> New (select publisher created earlier)
  
VS project:<br/>
 <ul>.NET Framework 4.7.1</ul>
 NuGet:<br/>
  <ul>Microsoft.CrmSdk.CoreAssemblies</ul>
  <ul>Microsoft.CrmSdk.XrmTooling.PluginRegistrationTool</ul>
 References:<br/>
  <ul>System.ServiceModel</ul>
  <ul>Microsoft.Xrm.Sdk.dll (this one comes from Microsoft.CrmSdk.XrmTooling.PluginRegistrationTool. packages\Microsoft.CrmSdk.CoreAssemblies.9.0.2.24\lib\net462)</ul>

Code:<br/>
  <ul>Implement 'IPlugin' intercafe</ul>
  <ul>example of default execute method: defaultExecution.txt</ul>
  
Build:<br/>
  <ul>Check: Properties -> Signing -> Sign the assembly</ul>
  <ul>Create new key (ex:key.snk)</ul>
  
Assign plugin:
  <ul>Use PluginRegistration.exe (packages\Microsoft.CrmSdk.XrmTooling.PluginRegistrationTool.9.1.0.14\tools)</ul>
