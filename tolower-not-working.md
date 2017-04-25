```
list = (from sr in dbContext.SERVICE_REQUEST
             join sc in dbContext.SERVICE_CUSTOMER on sr.CUSTOMER_ID equals sc.CUSTOMER_ID)
              where  (sr.SERVICE_REQUEST_NO.ToLower().Contains(objtobeAdvSearch.ServiceRequestNumber.ToLower()))
```






