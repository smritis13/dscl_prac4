# dscl_prac4
Structure in C
Structures (also called structs) are a way to group several related variables into one place. Each variable in the structure is known as a member of the structure.

Unlike an array, a structure can contain many different data types (int, float, char, etc.).
![image](https://user-images.githubusercontent.com/124857385/234312046-2113df4c-6296-4272-bc1d-ad1f1f91fa7b.png)


    #include <stdio.h>
    struct student {
        char name[50];
        int roll;
        float marks;
    } s;

    int main() {
        printf("Enter information:\n");
        printf("Enter name: ");
        fgets(s.name, sizeof(s.name), stdin);

        printf("Enter roll number: ");
        scanf("%d", &s.roll);
        printf("Enter marks: ");
        scanf("%f", &s.marks);

        printf("Displaying Information:\n");
        printf("Name: ");
        printf("%s", s.name);
        printf("Roll number: %d\n", s.roll);
        printf("Marks: %.1f\n", s.marks);

        return 0;
}<img width="372" alt="Screenshot 2023-04-07 192134" src="https://user-images.githubusercontent.com/124857385/230707816-88e7fa57-9376-4f46-a71f-87c3ef06e85d.png">
