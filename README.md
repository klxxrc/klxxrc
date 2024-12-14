scanf(",%", firstname);
 #include <stdio.h>
#include <string.h> 
int main() {
char username[] = "Basco";
char password[] = "Clark";
char inputuser[20], inputpass[20];
 
while (1) {
printf("Username: ");
scanf("%s", inputuser);
printf("Password: ");
scanf("%s", inputpass);
 

if (strcmp(inputuser, username) == 0 && strcmp(inputpass, password) == 0) {
printf("Login Successfully!!\n");
 
char lastname[100], firstname[100], middleInitial;
int age;
char course[10];
 
printf("Enter your last name: ");
scanf("%s", lastname);
 
printf("Enter your first name: ");

printf("Enter your middle initial: ");
scanf(" %c", &middleInitial);
 
printf("Enter your age: ");
scanf("%d", &age);
 
printf("\n======= Course Available [CCS] =======\n");
printf("BSIT\n");
printf("BSCS\n");
printf("ACT\n");
printf("======================================\n");
printf("Enter your course: ");
scanf("%s", course);
 
printf("\n==== YOUR INFORMATION =====\n");
printf("Last Name: %s\n", lastname);
printf("First Name: %s\n", firstname);
printf("Middle Initial: %c\n", middleInitial);
printf("Age: %d\n", age);
printf("Course: %s\n", course);
printf("======================================\n");
 
break;
} else {
printf("Invalid username/password\n");
}
}
 
return 0;
}
