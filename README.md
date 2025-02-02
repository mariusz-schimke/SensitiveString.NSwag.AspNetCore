# SensitiveString.NSwag.AspNetCore
[![NuGet Version](http://img.shields.io/nuget/v/SensitiveString.NSwag.AspNetCore.svg?style=for-the-badge&logo=nuget)](https://www.nuget.org/packages/SensitiveString.NSwag.AspNetCore/) [![NuGet Downloads](https://img.shields.io/nuget/dt/SensitiveString.NSwag.AspNetCore.svg?style=for-the-badge&logo=nuget)](https://www.nuget.org/packages/SensitiveString.NSwag.AspNetCore/)

This package extends [SensitiveString](https://www.nuget.org/packages/SensitiveString), ensuring that sensitive string types are correctly represented in Swagger/OpenAPI documentation.

## Example
If your API includes sensitive string types in requests or responses, this configuration ensures they are represented as standard strings in the generated OpenAPI documentation. 

```c#
// Program.cs
using TextPrivacy.SensitiveString.NSwag.AspNetCore;

builder.Services.AddOpenApiDocument(o =>
{
    // ...
    o.AddSensitiveStringSupport();
});
```