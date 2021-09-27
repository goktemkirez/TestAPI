# TestAPI .Net Core Web API

CREATE TABLE DBO.TestDepartment(
DepartmentId int identity(1,1),
DepartmentName nvarchar(500)
)

GO

INSERT INTO dbo.TestDepartment values ('IT')
INSERT INTO dbo.TestDepartment values ('Support')

GO

CREATE TABLE DBO.TestEmployee(
EmployeeId int identity(1,1),
EmployeeName nvarchar(500),
Department nvarchar(500),
DateOfJoining datetime,
PhotoFileName nvarchar(500)
)

GO

INSERT INTO dbo.TestEmployee values ('Bob', 'IT', GETDATE(), 'anonymous.png')

GO

Add SQL connection to: appsettings.json -> ConnectionStrings
