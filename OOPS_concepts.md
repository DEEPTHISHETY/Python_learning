OOPS concepts: Object oriented programming


    1. Class : Blueprint for creating objects
    2. Object  : Instance of CLass which will have attributes and behavior(methods)
    3. Encapsulation
    4. Inheritancr
    5. Polymorphism


Class and objects:

    class Student:    #Creating clss and class name should start with CAPS 
        name = "Deepthi Bhandary"
        roll_no = "50"
    
    S1 = Student()   #creating objects of clss : Student
    
    print(S1.name)   #accessing attributes of class using object

Constructor : Method iside a class [ __init__ function ]
All classes have a function called __init__ which will be executed when object is being initiated.

Program1:

    class Student:
            def __init__(self,fullname):         #constructor. Always take atleast one argument "self" pointing to object. Here S1
                    self.name = fullname
                
    S1 = Student("Deepthi Bhandary")
    print(S1.name)

    Output


progam2 : 

    class Student:
            def __init__(self,fullname):
                    self.fullname = fullname
                
    S1 = Student("Deepthi Bhandary")
    print(S1.fullname)

    Output : Deepthi Bhandary




