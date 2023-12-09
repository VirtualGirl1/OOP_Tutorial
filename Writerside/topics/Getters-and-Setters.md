# Getters and Setters

There are 2 types of variable a class can store.
Fields
 - variables that only store info and must be set when the class is created

Properties
 - Variable that can store data and ensure the value fits rules programed by the developer

Name - Here we want the name to be at least 2 letters long and not empty
```C#
    private string _name;

    public string Name 
    { 
        get 
        {
            return _name;   
        }
        set 
        {
            if (value == string.Empty || value.Length < 2) 
            {
                throw new Exception("Name must be at least 2 characters long");
            }
            
            _name = value;
        }
    }
    
    public int Age { get; set; }
```

notice that we have a 'private string _name'. This is because when we give get and set a body we need
another variable to store its value. 

With 'Age' we don't need to do this because get and set don't have a body, this is called an auto implemented property. 
When we build this, the builder adds creates its own body for get and set and adds a hidden '_age' field.
