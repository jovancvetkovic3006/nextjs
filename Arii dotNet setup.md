## Migration's LIST:
dotnet ef migrations list --context AriiContext --project Arii.Common --startup-project Arii.Common

## Migrate all pending:
dotnet ef database update --context AriiContext --project Arii.Common --startup-project Arii.Common

### ADD:
dotnet ef migrations add MarkerTypeEntity --context AriiContext --project Arii.Common --startup-project Arii.Common

### APPLY:
	dotnet ef database update --context AriiContext --project Arii.Common --startup-project Arii.Api

### REMOVE LATEST:
	dotnet ef migrations remove --context AriiContext --project Arii.Common --startup-project Arii.Api

### FE > BE connection
            connectionString = "Host=localhost;Port=5433;Database=arii;Username=arii;Password=ariipassword";

### Build
	dotnet build     

### Tests
	dotnet test Arii.Api.UnitTests
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5NzI5NzAzODAsMjEzMzc2ODMxOSw1Mj
U5MTU2MDQsMTk1MTgyODcxNCwtMTE4NzEyMTg5Nl19
-->