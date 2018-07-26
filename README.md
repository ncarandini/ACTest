# ACTest
A simple Hello World App made with Xamarin.Forms (.NET Standard) to test AppCenter Build task

Actually the issue with AppCenter is that the .NET Standard projects nedd to have a PackageReference (that shoudn't be needed), otherwise the Build Task of AppCenter fails. At the moment the workaround is to add `<PackageReference Include="NETStandard.Library" Version="2.0.3" />` to the `.csproj` file. No need to add this if building locally with VS 2017.
