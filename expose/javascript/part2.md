Problem 1. It prints *3*. Since i is declared as a var, which has a function scope, it undergoes 0->1->2->3(exit loop).

Problem 2. It prints *150*. Since discountedPrice is declared as a var, it can be updated. The newest value is prices[2]\*(1-discount)=300\*(0.5)=150.

Problem 3. It prints *150*. The newest finalPrice value is Math.round(150*100)/100=150. Math.round returns the value rounded to closest integer.

4. It returns *[50,100,150]*. The push function pushes the value to the end of array, so after the for loop discountedPrice=[50,100,150].

Problem 5. It causes an error because i is declared as a let within the for loop block, so it is not defined at line 12.

Problem 6. It causes an error because discountedPrice is declared as a let with block scope, so it is not defined at line 13.

Problem 7. It prints *150*. This time it doesn't cause error because line 14 is within the function block where finalPrice is defined.

Problem 8. It returns *[50,100,150]*. Since discounted is defined just within the function block, it gets updated and returned normally.

Problem 9. It causes an error because i is declared as let within the for loop block, so it is not defined at line 11.

Problem 10. It prints *3*.Since prices is passed as an array of length 3, length has a value of 3 and gets printed normally.

Problem 11. It returns *[50,100,150]*. Though discountedPrice is declared as a const and it cannot be reassigned, the push method does add the number to the array.(also explaining why 10 normally prints a value. If the push method cannot modify the const array, it will cause the error before printing 3 in problem 10)

Problem 12. A: student.name
    B: student["Grad Year"]
    C: student.greeting()
    D: student['Favorite Teacher'].name
    E: student.courseload[0]

Problem 13. A: 32, integers map to their exact string representation
    B: 1, char '3' is mapped to integer 3 because of minus
    C: 3, null is converted to 0
    D: "3null", null is converted to 'null'
    E: 4, true is converted to 1
    F: 0, false and null are converted to 0
    G: "3undefined", undefined is converted to "undefined"
    H: NaN, undefined is converted to NaN

Problem 14. A: true, as '2' is converted to 2
    B: false, as '2'>'12' in string comparison
    C: true, '2' is converted to 2
    D: false, === doesn't do type conversion
    E: false, true is converted to 1
    F: true, Boolean(2) equals true

Problem 15. == will do the type conversion. For instance (""==0) or (""==false) will return true. === will not do type conversion, so it will return false for the previous two comparisons.

Problem 17. It returns an array [2,4,6]. Function modifyArray iterates through every element in original array [1,2,3]. For the element, it is passed in doSomething and its product with 2 is pushed in newArr.

Problem 19. 1
    4
    3
    2
