```

	public IEnumerable<Customer> GetCustomers()
	{
		using(var context = new DBContext())
		{
			return from c in context.Customers
			       where c.Balance > 2000
			       select c;
		}
	}
	
```