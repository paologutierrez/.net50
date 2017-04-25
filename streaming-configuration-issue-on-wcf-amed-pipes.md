```
# Host Config
<services> 
    <service name="MyService"> 
        <endpoint address="net.pipe://localhost/MyService" 
                    binding="netNamedPipeBinding"bindingConfiguration="MyNamedPipeBinding"contract="MyApp.MyService" 
                    name="MyServiceEndpoint"/>
    </service> 
</services> 
<bindings> 
    <netNamedPipeBinding>
        <binding name="MyNamedPipeBinding" transferMode="StreamedResponse" 
                    maxBufferSize="32768" maxReceivedMessageSize="21474836480">
                    <security mode="None" />
        </binding> 
    </netNamedPipeBinding> 
</bindings> 

# Client config
<client> 
    <endpoint address="net.pipe://localhost/MyService" 
                    binding="netNamedPipeBinding"bindingConfiguration="MyNamedPipeBinding"contract="MyApp.MyService" 
                    name="MyServiceEndpoint">
    </endpoint>
</client> 
<bindings> 
    <netNamedPipeBinding>
        <binding name="MyNamedPipeBinding" transferMode="StreamedResponse" maxBufferSize="32768" 
                    maxReceivedMessageSize="21474836480">
            <security mode="None" /> 
        </binding> 
    </netNamedPipeBinding> 
</bindings> 
```