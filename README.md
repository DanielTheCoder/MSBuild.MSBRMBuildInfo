# MSBuild.MSBRMBuildInfo

[![Build status](https://ci.appveyor.com/api/projects/status/ehar1ei8n2d075rx?svg=true)](https://ci.appveyor.com/project/DanielTheCoder/msbuild-msbrmbuildinfo)

MSBuild.MSBRMBuildInfo (MSBuild Release Management Build Info) is a simple solution to enable Application Insights deployment markers in an application without manually editing MSBuild files.
  
... *Application Insights is a set of services that integrates production monitoring data with development tools.* ...
from [Implementing Deployment Markers in Application Insights](http://blogs.msdn.com/b/visualstudioalm/archive/2013/11/14/implementing-deployment-markers-in-application-insights.aspx)

How to use  
---------------------
Install nuget package MSBuild.MSBRMBuildInfo

How does it work?
---------------------
Instead of manually setting the required MSBuild properties in your project you can install this nuget package which will add a MSBuild file with the required properties already set  
```csharp
<PropertyGroup> 
    <!-- Generate the BuildInfo.config file --> 
    <GenerateBuildInfoConfigFile>true</GenerateBuildInfoConfigFile> 
    <IncludeServerNameInBuildInfo>true</IncludeServerNameInBuildInfo> 
    <VisualStudioVersion>12.0</VisualStudioVersion> 
</PropertyGroup>
```

Related MSBuild targets
-------------------
C:\Microsoft\VisualStudio\v12.0\BuildInfo\Microsoft.VisualStudio.ReleaseManagement.BuildInfo.Targets

------------
If you are interested in contributing,  
  
1. Get a Github account  
1. Fork the project  
1. Make your feature addition or bugfix. Please also update the [changelog](https://github.com/DanielTheCoder/MSBuild.MSBRMBuildInfo/blob/master/changelog.txt).  
1. Send me a pull request via GitHub  