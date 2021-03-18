# Calendar-Generator-
Algorithim of the goes as:
Note : Program Starts from  main function (int main()) 

Step-1  We take the year(century) from user as int value and store it in  'year'

Step-2  We take the month (as jan ,feb...) as string and store it in 'month'

Step-3  we form an array (arr) of months  as(arr[]={"jan","feb","mar","apr","may","jun","jul","aug","sep","oct","nov","dec"}

step-4  Then we compare month entered by the user with all the elements of above array using for loop and if the entered month matches then we assign the value of varailble 'n'
        the index of entered month in array (for eg : for jan . n=0, feb, n=1 and so on..for dec n=11)
        
step-5  Now switch cases are  formed for all the months with 'n' as argument of switch (switch(n)) hence if user entered "mar" (March ) then n=2(from above step we got the 
        value of n ) and we will be forwarded to case(2) and all the instructions under case(2) will be executed .  
       
        

Step-6  in each case first we call a function first_day which will return first day of the entered month in the from of integer from 0-6 such that 0 represents Sunday , 1-monday 
        and so on till 6- Saturday . Hence if the function returns 1 the first day of the month is Monday.
        This returned int value is stored in int variable 'Ist_day'.
         Note: zellar's rule has been used to find first day of the month. (https://www.careeranna.com/articles/find-day-for-given-date-quickly/)

Step -7 Now we know the day(Sun-Sat) from which our calendar will start so all we need to do now is print the dates  starting  from the first day and then print all the
        dates till the last day of the entered month (i.e 30 or 31 or 29 or 28)
        So for printing the calendar we call a function display_calendar and pass the name of month, first day of month and no. of days in entered month
        
