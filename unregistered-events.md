```
 
Order newOrder=new Order
(“EURUSD”, DealType.Buy, Price ,PriceTolerance, TakeProfit, StopLoss);

newOrder.OnPlaced+=OrderPlaced;
m_PendingDeals.Add(newOrder);
```