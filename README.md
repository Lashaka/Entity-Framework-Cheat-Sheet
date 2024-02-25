# Entity Framework Cheat Sheet
 

## Common commands
Remove-Migration: Removes the last migration.
Add-Migration "Migration-Name" -OutputDir "MigrationsFolder": Specifies the folder where migrations should be generated.
Update-Database -TargetMigration "TargetMigrationName": Updates the database to a specific migration.
Update-Database -Script: Generates a SQL script of the pending migrations.
Enable-Migrations: Enables migrations for the project.
Add-Migration "Migration-Name" -IgnoreChanges: Adds a migration without changes to the model.


## Establish Connection String
" <connectionStrings>
   <add name="MyDbContext" connectionString="YourConnectionStringHere" providerName="System.Data.SqlClient" />
 </connectionStrings>"


## DAL (data access layer) and web project heirarchy
1-  Set web project as Set as Startup Project

2- In Package Manager Console, set data access layer as a default project

3- now i can run commands in the right heirarchy