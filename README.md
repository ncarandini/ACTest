# ACTest
A simple Hello World App made with Xamarin.Forms (.NET Standard) to test AppCenter Build task

Actually I see two issue:

1. The .NET Standard projects nedd to have a PackageReference (that shoudn't be needed), otherwise the Build Task of AppCenter fails:
<PackageReference Include="NETStandard.Library" Version="2.0.3" />

2. When using ProGuard, even if the build process succeeded, the Adoid APK fails to run on Andoid devices (on emulator and real device).
