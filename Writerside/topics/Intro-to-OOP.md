# Intro to OOP

OOP Stands for Object-Oriented Programing, a type of programming that
uses class to define different aspects of a piece of software

---

Here is an example of a class that describes a person
```C#
    class Person 
    {
        public string name;
        public int age;
        public string hairColor;
        
        public void Walk();
        public void Talk(string msg);
    };
```

Here we define the class of person
```C#
    class Person
```

Below that we define a few fields that are a part of the class
```C#
    public string name;
    public int age;
    public string hairColor;
```

And finally some methods to describe actions to take
```C#
    public void Walk();
    public void Talk(string msg);
```

The first method 'Walk()' takes no arguments and returns nothing

The second method 'Talk()' takes one argument, a string for the person to say
and returns nothing