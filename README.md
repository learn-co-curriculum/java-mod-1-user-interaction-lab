# User Interaction Lab

## Learning Goals

- Take user input
- Process and display user input

## Instructions

Let's go back to our `Student` class example!

```java
public class Student {
    private String name;
    
    Student(String name) {
        this.name = name;
    }
    
    public String getName() {
        return name;
    }
    
    public void setName(String name) {
        this.name = name;
    }

    /**
     * Take in a student numeric grade and provide feedback
     * on how they did on a test
     * @param grade : int - numeric grade the student received
     *                on the test
     */
    public void calculateGrade(int grade) {
        if (grade >= 70) {
            System.out.println("Congrats! You passed!");
            if (grade >= 90) {
                System.out.println("Wow! You got an A!");
            }
        } else {
            System.out.println("Oops! Better luck next time!");
        }
    }
    
    public static void main(String args[]) {
        // Write Student user input here
    }
}
```

Let's ask the user for input and use our `Student` class! 

First, prompt the user for their name and then create a `Student` instance with
that name.

Second, greet the user by saying, "Hi <name>! What grade did you get on the
test?" This will prompt the user to enter in an integer value for a grade.

Third, call the method `calculateGrade()` which will print a message based on
the grade the user typed in.
