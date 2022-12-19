# praktikum-9

Assert Statement

           def KelvinToFahrenheit(Temperature):
              assert (Temperature >= 0),"Colder than absolute zero!"
              return ((Temperature-273)*1.8)+32
           print (KelvinToFahrenheit(273))
           print (int(KelvinToFahrenheit(505.78)))
           print (KelvinToFahrenheit(-5))
         
![image](https://user-images.githubusercontent.com/115523263/208497551-83cb17f4-5933-4c1b-a24e-525045f66e18.png)

Clause

    try:
        fh = open("testfile", "w")
        fh.write("This is my test file for exception handling!!")
    except IOError:
        print ("Error: can\'t find file or read data")
    else:
        print ("Written content in the file successfully")
        fh.close()
    
![image](https://user-images.githubusercontent.com/115523263/208497659-bbca81e6-41e9-48d2-b7e6-013229060a1d.png)

Exception Statement

    try:
        fh = open("testfile", "r")
        fh.write("This is my test file for exception handling!!")
    except IOError:
        print ("Error: can\'t find file or read data")
    else:
        print ("Written content in the file successfully")
        fh.close()
    
![image](https://user-images.githubusercontent.com/115523263/208497802-6fac839b-2f6c-4219-8a7e-144f37347ff5.png)

Try-finally clause

    try:
        fh = open("testfile", "r")
        try:
            fh.write("This is my test file for exception handling!!")
        finally:
            print("going to close the file")
            fh.close()
    except IOError:
        print ("Error: can\'t find file or read data")

![image](https://user-images.githubusercontent.com/115523263/208499667-0fb98d39-2587-4649-a06a-9b041df2eac2.png)

exception argument

    def temp_convert(var):
        try:
            return int(var)
        except ValueError(Argument):
            print("the argument does not contain numbers\n",Argument)

    temp_convert("xyz")

![image](https://user-images.githubusercontent.com/115523263/208500470-4f7b95e0-e4b5-4b3a-96af-fb35c2db6efa.png)

Raise

    def functionName( level ):
        if level < 1:
            raise ("Invalid level!", level)
        
![image](https://user-images.githubusercontent.com/115523263/208500870-109d94f1-86f4-47d0-bd24-8437f2dbe37f.png)

User Defined

    class Networkerror(RuntimeError):
        def __init__(self, arg):
            self.args = arg
    try:
        raise Networkerror("Bad hostname")
    except Networkerror(e):
        print(e.args)
    
![image](https://user-images.githubusercontent.com/115523263/208504210-02739b9e-7d84-4eb7-8343-2948f349d4e2.png)
