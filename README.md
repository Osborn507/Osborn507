- 👋 Hi, I’m @Osborn507
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Osborn507/Osborn507 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

#include<stdio.h>

int main(int argc, char *argv[]) {
    int n = (int)(*argv[1] - '0');
    for(int i = 0; i<n ;i++){
        char name[100];
        char dept[100];
        float annual_income = 0.0;
        printf("Enter the details of %dth employee, Name, dept and annual income\n", i + 1);
        scanf("%s\n%s\n%f", name, dept, &annual_income);

        if(annual_income <= 50000){
            annual_income += (annual_income/10.0);
        }
        else if(annual_income <= 100000){
            annual_income += (annual_income/5.0);
        }
        printf("Details of %dth Employee\n Name:%s\nDept:%s\nAnnual income:%f\n", i + 1, name, dept, annual_income);
    }
}
