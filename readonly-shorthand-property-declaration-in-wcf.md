```

//Data Contract attribute applied to class to make it available to client.

//Data Member attribute applied to the 'MyVar' readonly property.

    [DataContract]
    public class MyValueObject
    {
        [DataMember]
        public int MyVar
        {
            get;
        //This will not work, as WCF needs both getter and setter to access property.

        }
    }  

    //Correct version with both getters and setter defined.

    [DataContract]
    public class MyValueObject
    {
        [DataMember]
        public int MyVar
        {
            get; 
            set {}
            //Empty setter block is supplied for readonly property. 

        }
    }
    
```