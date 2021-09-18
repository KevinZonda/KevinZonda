![](img/banner-x.png)
```csharp
using ADT;
using System.Linq;

public static class KevinZonda
{
    public static BasicInfo BasicInfo => new()
    {
        Name        = "Kevin CHEN",
        PGP         = "867C 7D44 DFDF 603A C971 8505 6FF4 CDC2 D404 9C0A",
        Gender      = Gender.Male,
        Location    = "Birmingham, West Midlands, United Kingdom",
        Languages   = new[] { "zh-CN", "en-GB" },
        ContactInfo = new()
        {
            Emails = new[]
            {
                "realkevin#tutanota.com",
                "kevin#fastgit.org",
                "kevin#v2fly.org",
                "kevin#alumni.hmuniversity.org",
                "kevin#is-rbq.com"
            }.Select(x => x.Replace("#", "@")).ToArray(),
            Others = new()
            {
                { "Telegram", new[] { "KevinZonda"  } }, // https://t.me/KevinZonda
                { "Twitter" , new[] { "FailedWaste" } }  // https://twitter.com/FailedWaste
            }
        }
    };

    public static DevInfo DevInfo => new()
    {
        Environments = new[] { "Windows10x64", "Debian10x64" },
        Tools        = new[] { "IDEA", "Rider", "Visual Studio 2017", "Visual Studio Code" },
        Languages    = new[] { "C#", "Go", "Java" },
        Projects     = new[] { "FastGit UK", "PassCore" }
    };
}
```
