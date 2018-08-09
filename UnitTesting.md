# Writing unit tests

```csharp
public Customer GetCustomerById(int id)
```

> For the above method, the correct way to write unit tests:

```csharp
[UnitOfWork_StateUnderTest_ExpectedBehavior]

GetCustomerById_WithValidId_ReturnsCustomer
GetCustomerById_WithInvalidId_ReturnsNull
```

Link: https://stackoverflow.com/questions/20874768/how-do-you-name-your-unit-test-methods?noredirect=1&lq=1
