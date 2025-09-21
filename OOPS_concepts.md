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

    Output : Deepthi Bhandary 


progam2 : 

    class Student:
            def __init__(self,fullname):
                    self.fullname = fullname      # you can use the same name for passed argument to constructor and variable used inside constructor
                
    S1 = Student("Deepthi Bhandary")
    print(S1.fullname)

    Output : Deepthi Bhandary


Class and Instance attributes: If class attr and object attr name is same then object attribute will take the precedence

    class Student:
        college_name = "Managlore College"  # Class attributes which is common for all objects. 
                                            #can be access directly used class attribute or object attribute
        def __init__(self, fullname, roll_no):
            self.name = fullname   # Object attributes
            self.roll_no = roll_no  #Object attibutes
                    
    S1 = Student("Deepthi Bhandary", 50)
    print(S1.name)
    print(S1.roll_no)
    print("Student name from object attribute:",S1.college_name)
    print("student name from class attribute:",Student.college_name)

    Output:-

    Deepthi Bhandary
    50
    Student name from object attribute: Managlore College
    student name from class attribute: Managlore College


Assignment: - Create a student class that takes name and marks of 3 subjects as an arguments in constructor. then create a method to print the average

    class Student:
    
        def __init__(self, name, math_marks, science_marks, physics_marks):
            self.name = name
            self.math_marks = math_marks
            self.science_marks = science_marks
            self.science_marks = science_marks
    
        def avergae_marks(self):
            self.average = (self.math_marks + self.science_marks + self.science_marks) / 3
            print("Hi", self.name,"your average is:",self.average)
        
    S1 = Student("Deepthi bhandary", 100, 50, 90)
    S1.avergae_marks()

    Output : Hi Deepthi bhandary your average is: 66.66666666666667




