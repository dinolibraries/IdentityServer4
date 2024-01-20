dotnet sln FullpackISV4.sln add **/*.csproj
FOR /R %i IN (*.csproj) DO dotnet sln add "%i"

dotnet sln FullpackISV4.sln add (ls -r src/**/*.csproj)
./FullpackISV4.sln