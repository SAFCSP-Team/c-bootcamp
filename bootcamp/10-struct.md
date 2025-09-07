# Struct

Imagine you want to store details about a person, like name (string), age (integer), and height (float). Instead of creating separate variables for each attribute, you can group them together using a `struct`.

### Defining a Structure
```c
struct struct_name{
    data_type variable_name;
    data_type variable_name;
};
```
* struct: A keyword to define a structure.
* struct_variable_name: The name of the structure.
* variable_name: Variables (or members) within the structure, which can be of different data types.
  
```c
struct Person {
    char name[50];
    int age;
    float height;
};
```
> Note: In C, strings are represented as character arrays because the language does not have a built-in string data type.

### Using a Structure
To use a structure, use the struct keyword within the `main()` function, followed by the structure's name and then the variable name for the structure.
```c
struct struct_name{
    data_type variable_name;
    data_type variable_name;
};

int main() {
  struct struct_name struct_variable_name;
  return 0;
}
```

### typedef struct
If we use the `typedef` keyword, it allows the structure to be referenced using an alias name instead of the struct name.
```c
typedef struct struct_name {
    data_type variable_name;
    data_type variable_name;
} typedefName; // This is the new alias


int main() {
 typedefName struct_variable_name;
  return 0;
}
```

## Example
- Create a Person struct
```c
#include <stdio.h>
#include <string.h> 

struct Person {
    char name[50];
    int age;
    float height;
};

int main() {
    struct Person person1;  // Declare a variable of type struct Person

    strcpy(person1.name, "Sultan"); // Assign a value to the string using the strcpy function
    person1.age = 30;             // Assign integer to age
    person1.height = 170.7;         // Assign float to height

    // Print the values
    printf("Name: %s\n", person1.name);
    printf("Age: %d\n", person1.age);
    printf("Height: %.1f\n", person1.height);

    return 0;
}
```

Output
```
Name: Sultan
Age: 30
Height: 170.7
```



- Create a Person struct using a `typedef keyword`.
```c
typedef struct Person {
    char name[50];
    int age;
    float height;
} PersonInfo;
```

```c
#include <stdio.h>
#include <string.h>

// Define struct Person and create an alias PersonInfo
typedef struct Person {
    char name[50];
    int age;
    float height;
} PersonInfo;

int main() {
    PersonInfo person1;  // Declare a variable of type PersonInfo

    // Assign values to the structure members
    strcpy(person1.name, "Sultan");
    person1.age = 30;
    person1.height = 170.7;

    // Print the values
    printf("Name: %s\n", person1.name);
    printf("Age: %d\n", person1.age);
    printf("Height: %.1f\n", person1.height);

    return 0;
}
```

## Practice
1. Define a structure called `Employee` with:
* `id` (integer)
* `name` (string)
* `salary` (float)
  
2. Declare a variable of type `struct` Employee.

3. Assign values and print the details.
```c
#include <stdio.h>

int main() {

    return 0;
}
```
