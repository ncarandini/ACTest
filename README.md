# ACTest
A simple Hello World App made with Xamarin.Forms (.NET Standard) to test AppCenter Build task

Actually I see two issue:

1. The .NET Standard projects nedd to have a PackageReference (that shoudn't be needed), otherwise the Build Task of AppCenter fails. I've solved adding `<PackageReference Include="NETStandard.Library" Version="2.0.3" />` to the `.csproj` file but it's only a workaround. No need to add this if building locally on my PC with VS 2017.

2. When using ProGuard, even if the build process succeeded, the Adoid APK fails to run on Andoid devices (on emulator and real device).
