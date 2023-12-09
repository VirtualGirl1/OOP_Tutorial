# Inheritance

Take the 'Person' class defined before. What do we do when we have a similar class,
like Teacher and Student, that have the same properties as person as well as a few more

In this case we use inheritance. Take the following classes:
```C#
class Teacher : Person 
{
    public string subject;
    public int patience;
    public List<Student> students;
    
    public void Teach();

};

class Student : Person 
{
    public int grade;
    
     
    public void Learn(string lesson);
};
```

