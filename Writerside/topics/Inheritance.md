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

Here, both Teacher and Student have access to all the fields from Person,
as well as the methods 'Walk()' and 'Talk()'

In 'Teacher' we add 3 new fields to represent the subject, their level of patience,
and a list of the students they teach. It also has a new method called 'Teach()'.

In 'Student' we only add one field 'grade' and a method called 'Learn()' which takes the lesson.
