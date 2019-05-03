# student-management-system
To insert delete and update the student information.
source code:
#include<stdio.h>
#include<conio.h>
#include<graphics.h>
#include<dos.h>
void std1(void);
void std2(void);
void std3(void);
void std4(void);
void std5(void);
void std6(void);
void std7(void);
void std8(void);
void main(void)
{
clrscr();
int gd=DETECT,gm;
initgraph(&gd,&gm,"c:\\TC\\BGI");
setbkcolor(RED);
union REGS i,o;
i.x.ax=1;
int86(0x33,&i,&o);


 int a[8]={120,121,123,124,125,126,127,128};
 char r;
 //printf(" = ");
 //scanf("%d",&a);
 printf("\n\t1.--See detail for Roll no  120 ");
 printf("\n\t2.--See detail for Roll no  121 ");
 printf("\n\t3.--See detail for Roll no  123 ");
 printf("\n\t4.--See detail for Roll no  124 ");
 printf("\n\t5.--See detail for Roll no  125 ");
 printf("\n\t6.--See detail for Roll no  126 ");
 printf("\n\t7.--See detail for Roll no  127 ");
 printf("\n\t8.--See detail for Roll no  128 ");
 printf("\n\t Choose roll No = ");
 scanf("%d",&a[8]);
 switch(a[8])
  {
  case 120:
  std1();
  break;
  case 121:
  std2();
  break;
  case 123:
  std3();
  break;
  case 124:
  std4();
  break;
  case 125:
  std5();
  break;
  case 126:
  std6();
  break;
  case 127:
  std7();
  break;
  case 128:
  std8();
  break;

   }

  printf("\n Do you want other information(Y/N)");
   scanf("%s",&r);
   switch(r)
   {
  case'y':
   main();
  break;
   case'n':

   break;
   }

   getch();

closegraph();
   }
   void std1(void)
   {
   int b,p;
   printf("\n\t Enter Student Password | ");
   scanf(" %d ",&p);
   switch(p)
   {
   case 1111:
  printf(" \nSTUDENT NAME : MUHAMMAD TALHA ");
  printf(" \nFATHER NAME  : MUHAMMAD JABBAR ");
  printf("\n\n Press 1 For Student Personal Information = \n Press 2 For Student Education = ");
  scanf("%d",&b);
  switch(b)
   {
   case 1:
 //if(a>0 && a<2)
   printf("\n Student Personal Information \n ******* ******** ***********");
   printf("\n Gender          :  Male");
   printf("\n Country         :  Pakistan ");
   printf("\n Religion        :  Islam ");
   printf("\n N.I.C No        :  1890 - 4356345 - 6 ");
   printf("\n Passport no     :  31195855 ");
   printf("\n Married/Single  :  Single ");
   printf("\n Blood Group     :  B+ ");

   break;
   case 2:

  // if (a>1 && a<3)
   printf("\n Student Education Report \n ******* ********* ******");
   printf("\n Student Of      :  SE,1st semster ");
   printf("\n Dues            :  128 $ ");
   printf("\n Matric          :  A+ Grade 82% ");
   printf("\n Intermediate    :  A Grade 79% ");
   printf("\n Session Report  :  Good ");
   printf("\n Semster Report  :  All clear ");
   printf("\n    GPA          :  3.2 ");
   printf("\n Decipline       :  Nice person ");

  break;
   }
  break;
  default:
  printf("\n <<< Incorrect Password >>> ");
  break;

   }
   }
    void std2(void)
   {
   int c,p;
    printf("\n Enter Student Password | ");
   scanf(" %d ",&p);
   switch(p)
   {
   case 2222:
  printf(" \n Student Name   |  Sarib Bin Iqbal ");
  printf(" \n Father Name    |  MUHAMMAD Ibqal ");
  printf("\n\n Press 1 For Student Personal Information = \n Press 2 For Student Education = ");
  scanf("%d",&c);
  switch(c)
  {
  case 1:
 //if(a>0 && a<2)
   printf("\n Student Personal Information \n ******* ******** ***********");
   printf("\n Gender          :  Male");
   printf("\n Country         :  India ");
   printf("\n Religion        :  Islam ");
   printf("\n N.I.C No        :  1890 - 4356 - 6123 ");
   printf("\n Passport no     :  1985324 ");
   printf("\n Married/Single  :  Single ");
   printf("\n Blood Group     :  O+ ");
   // else
 // printf("\n For More Detail Press  ");
   break;
   case 2:
 // if(a>1 && a<3)
   printf("\n Student Education Report \n ******* ********* ******");
   printf("\n Student Of      :  SE,1st semster ");
   printf("\n Dues            :   Nill ");
   printf("\n Matric          :  A Grade 74% ");
   printf("\n Intermediate    :  C Grade 54% ");
   printf("\n Session Report  :  Not Good ");
   printf("\n Semster Report  :  All clear ");
   printf("\n    GPA          :  2.4 ");
   printf("\n Decipline       :  Good person ");
   // else
   break;
  }
  break;
  default:
  printf("\n <<< Incorrect Password >>> ");
  break;
  }
  }
  void std3(void)
   {
   int c,p;
    printf("\n Enter Student Password | ");
   scanf(" %d ",&p);
   switch(p)
   {
   case 3333:
  printf(" \n Student Name   |  Huma Butt ");
  printf(" \n Father Name    |  Nazir Muhammad");
  printf("\n\n Press 1 For Student Personal Information = \n Press 2 For Student Education = ");
  scanf("%d",&c);
  switch(c)
  {
  case 1:
 //if(a>0 && a<2)
   printf("\n Student Personal Information \n ******* ******** ***********");
   printf("\n Gender          :  Female");
   printf("\n Country         :  Saudia Arabia ");
   printf("\n Religion        :  Islam ");
   printf("\n N.I.C No        :  0256 - 5634356 - 00 ");
   printf("\n Passport no     :  6297824 ");
   printf("\n Married/Single  :  Married ");
   printf("\n Blood Group     :  A+ ");
   // else
 // printf("\n For More Detail Press  ");
   break;
   case 2:
 // if(a>1 && a<3)
   printf("\n Student Education Report \n ******* ********* ******");
   printf("\n Student Of      :  MSc, final Year ");
   printf("\n Dues            :   Nill ");
   printf("\n Matric          :  B Grade 67% ");
   printf("\n Intermediate    :  A Grade 73% ");
   printf("\n Session Report  :  Good ");
   printf("\n Semster Report  :  All clear ");
   printf("\n    GPA          :  3.0 ");
   printf("\n Decipline       :  Excellent ");
   // else
   break;
  }
  break;
  default:
  printf("\n <<< Incorrect Password ");
  break;
   }
   }
   void std4(void)
   {
   int c,p;
    printf("\n Enter Student Password | ");
   scanf(" %d ",&p);
   switch(p)
   {
   case 4444:
  printf(" \n Student Name   |  Hamza ");
  printf(" \n Father Name    |  Muhammad Siddique");
  printf("\n\n Press 1 For Student Personal Information = \n Press 2 For Student Education = ");
  scanf("%d",&c);
  switch(c)
  {
  case 1:
 //if(a>0 && a<2)
   printf("\n Student Personal Information \n ******* ******** ***********");
   printf("\n Gender          :  Male");
   printf("\n Country         :  Saudia Arabia ");
   printf("\n Religion        :  Islam ");
   printf("\n N.I.C No        :  0256 - 5634356 - 00 ");
   printf("\n Passport no     :  6297824 ");
   printf("\n Married/Single  :  Married ");
   printf("\n Blood Group     :  A+ ");
   // else
 // printf("\n For More Detail Press  ");
   break;
   case 2:
 // if(a>1 && a<3)
   printf("\n Student Education Report \n ******* ********* ******");
   printf("\n Student Of      :  MSc, final Year ");
   printf("\n Dues            :   Nill ");
   printf("\n Matric          :  B Grade 67% ");
   printf("\n Intermediate    :  A Grade 73% ");
   printf("\n Session Report  :  Good ");
   printf("\n Semster Report  :  All clear ");
   printf("\n    GPA          :  3.0 ");
   printf("\n Decipline       :  Excellent ");
   // else
   break;
  }
  break;
  default:
  printf("\n <<< Incorrect Password ");
  break;
   }
   }
      void std5(void)
   {
   int c,p;
    printf("\n Enter Student Password | ");
   scanf(" %d ",&p);
   switch(p)
   {
   case 5555:
  printf(" \n Student Name   |  Ritka Sharma ");
  printf(" \n Father Name    |  Sharma");
  printf("\n\n Press 1 For Student Personal Information = \n Press 2 For Student Education = ");
  scanf("%d",&c);
  switch(c)
  {
  case 1:
 //if(a>0 && a<2)
   printf("\n Student Personal Information \n ******* ******** ***********");
   printf("\n Gender          :  Female");
   printf("\n Country         :  India ");
   printf("\n Religion        :  India ");
   printf("\n N.I.C No        :  0256 - 5456 - 2090 ");
   printf("\n Passport no     :  0091192 ");
   printf("\n Married/Single  :  Single ");
   printf("\n Blood Group     :  B- ");
   break;

   case 2:
   printf("\n Student Education Report \n ******* ********* ******");
   printf("\n Student Of      :  CE, 2nd Year ");
   printf("\n Dues            :   Nill ");
   printf("\n Matric          :  A Grade 73% ");
   printf("\n Intermediate    :  D Grade 46% ");
   printf("\n Session Report  :  Not well ");
   printf("\n Semster Report  :  Paper fail in 2nd Semster");
   printf("\n    GPA          :  2.0 ");
   printf("\n Decipline       :  Normal ");
   // else
   break;
  }
  break;
  default:
  printf("\n <<< Incorrect Password ");
  break;
   }
   }
   void std6(void)
   {
   int c,p;
    printf("\n Enter Student Password | ");
   scanf(" %d ",&p);
   switch(p)
   {
   case 6666:
  printf(" \n Student Name   |  John Melton ");
  printf(" \n Father Name    |  Boil Melton");
  printf("\n\n Press 1 For Student Personal Information = \n Press 2 For Student Education = ");
  scanf("%d",&c);
  switch(c)
  {
  case 1:
 //if(a>0 && a<2)
   printf("\n Student Personal Information \n ******* ******** ***********");
   printf("\n Gender          :  Male");
   printf("\n Country         :  Canada ");
   printf("\n Religion        :  Nill ");
   printf("\n N.I.C No        :  1598-478912750-2019 ");
   printf("\n Passport no     :  9912288 ");
   printf("\n Married/Single  :  Single ");
   printf("\n Blood Group     :  A- ");
   break;

   case 2:
   printf("\n Student Education Report \n ******* ********* ******");
   printf("\n Student Of      :  SE, 2nd Year ");
   printf("\n Dues            :   1349 $ ");
   printf("\n Matric          :  A+ Grade 83% ");
   printf("\n Intermediate    :  A+ Grade 86% ");
   printf("\n Session Report  :  Excellent ");
   printf("\n Semster Report  :  Very Good");
   printf("\n    GPA          :  3.9 ");
   printf("\n Decipline       :  Nice");
   // else
   break;
  }
  break;
  default:
  printf("\n <<< Incorrect Password ");
  break;
   }
   }
   void std7(void)
   {
   int c,p;
    printf("\n Enter Student Password | ");
   scanf(" %d ",&p);
   switch(p)
   {
   case 7777:
  printf(" \n Student Name   |  Sehar Butt");
  printf(" \n Father Name    |  Muhammad Butt");
  printf("\n\n Press 1 For Student Personal Information = \n Press 2 For Student Education = ");
  scanf("%d",&c);
  switch(c)
  {
  case 1:
 //if(a>0 && a<2)
   printf("\n Student Personal Information \n ******* ******** ***********");
   printf("\n Gender          :  Female");
   printf("\n Country         :  Pakistan ");
   printf("\n Religion        :  Islam ");
   printf("\n N.I.C No        :  1598-289452-2 ");
   printf("\n Passport no     :  097791 ");
   printf("\n Married/Single  :  Single ");
   printf("\n Blood Group     :  O+ ");
   break;

   case 2:
   printf("\n Student Education Report \n ******* ********* ******");
   printf("\n Student Of      :  SE, 4th Year ");
   printf("\n Dues            :  13 $ ");
   printf("\n Matric          :  B Grade 63% ");
   printf("\n Intermediate    :  A+ Grade 81% ");
   printf("\n Session Report  :  Excellent ");
   printf("\n Semster Report  :  Very Good");
   printf("\n    GPA          :  3.1 ");
   printf("\n Decipline       :  Nice");
   // else
   break;
  }
  break;
  default:
  printf("\n <<< Incorrect Password ");
  break;
   }
   }

   void std8(void)
   {
   int c,p;
    printf("\n Enter Student Password | ");
   scanf(" %d ",&p);
   switch(p)
   {
   case 8888:
  printf(" \n Student Name   |  Syed Ali Hussain ");
  printf(" \n Father Name    |  Muhammad Hussain");
  printf("\n\n Press 1 For Student Personal Information = \n Press 2 For Student Education = ");
  scanf("%d",&c);
  switch(c)
  {
  case 1:
 //if(a>0 && a<2)
   printf("\n Student Personal Information \n ******* ******** ***********");
   printf("\n Gender          :  Male");
   printf("\n Country         :  Pakistan ");
   printf("\n Religion        :  Islam ");
   printf("\n N.I.C No        :  1096-982315-0 ");
   printf("\n Passport no     :  0091212 ");
   printf("\n Married/Single  :  Single ");
   printf("\n Blood Group     :  B- ");
   break;

   case 2:
   printf("\n Student Education Report \n ******* ********* ******");
   printf("\n Student Of      :  SE, 1st Year ");
   printf("\n Dues            :   All Clear ");
   printf("\n Matric          :  A Grade 73% ");
   printf("\n Intermediate    :  A Grade 71% ");
   printf("\n Session Report  :  Good ");
   printf("\n Semster Report  :  Excellent");
   printf("\n    GPA          :  2.9 ");
   printf("\n Decipline       :  Awesome");
   // else
   break;
  }
  break;
  default:
  printf("\n <<< Incorrect Password ");
  break;
   }
   }
