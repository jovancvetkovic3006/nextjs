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
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTkxMTQ4MDk2MCwyMTMzNzY4MzE5LDUyNT
kxNTYwNCwxOTUxODI4NzE0LC0xMTg3MTIxODk2XX0=
-->