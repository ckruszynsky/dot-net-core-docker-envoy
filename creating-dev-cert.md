# Creating https certs for projects

To create the https certs for the project run the following command in the terminal :

    dotnet dev-certs https -ep $env:USERPROFILE\.aspnet\https\CoffeeAPI.pfx -p pa55w0rd!

    dotnet dev-certs https -ep $env:USERPROFILE\.aspnet\https\TeaAPI.pfx -p pa55w0rd!

## Tell .net to trust dev-certs

Make sure to run the following command after the above commands to ensure you are trusting
dev-certs

    dotnet dev-certs https -trust

# Where are certs stored

To check to make sure your certs were indeed generated go to the following path to ensure
the .pfx files exist

        C:\Users\<Username>\.aspnet\https

You should see your .pfx that were created listed here.
