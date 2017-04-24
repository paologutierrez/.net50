```

public class UserService
{
    private readonly IMessagingService _messagingService;
    public UserService(IMessagingService messagingService)
    {
        _messagingService = messagingService;
    }

    public bool RegisterUser(string login, string emailAddress, string password)
    {
        // insert user to the database

        // generate an activation code to send via email

        // save activation code to the database

        // create an email message object
        try
        {
            _messagingService.SendRegistrationEmailMessage(message);
        }
        catch (Exception)
        {
            // boom!
        }
        return true;

    }
}

```