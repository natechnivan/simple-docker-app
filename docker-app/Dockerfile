FROM mcr.microsoft.com/dotnet/core/sdk:3.1
WORKDIR /app

# Copy everything else and build
COPY . .

# Build runtime image
ENV ASPNETCORE_URLS http://*:8082
EXPOSE 80
ENTRYPOINT ["dotnet", "docker-app.dll"]