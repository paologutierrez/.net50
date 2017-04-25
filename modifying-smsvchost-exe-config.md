```
<net.tcp listenBacklog=”10″ maxPendingConnections=”100″ maxPendingAccepts=”2″ receiveTimeout=”00:00:10″ teredoEnabled=”false”>
    <allowAccounts>
        // LocalSystem account
        <add securityIdentifier=”S-1-5-18″/>

        // LocalService account
        <add securityIdentifier=”S-1-5-19″/>
       
        // Administrators account
        <add securityIdentifier=”S-1-5-20″/>
       
        // Network Service account
        <add securityIdentifier=”S-1-5-32-544″ />
       
        // IIS_IUSRS account (Vista only)
        <add securityIdentifier=”S-1-5-32-568″/>
    </allowAccounts>
</net.tcp>

```
