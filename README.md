# TestItem_Mindbox
My first repository on GitHub.

**Test item:**<br />
There is a form on the website that calculates the possibility of obtaining a Russian passport based on age, in accordance with current legislation.
The field accepts integers between 0 and 115, inclusive, as input. Based on this input, we receive one of three possible messages: "Impossible to issue", "Possible to issue" or "Error".<br />

Necessary:
1. Divide the input data using the technique of boundary values and determine the result for each case;
2. Divide the input data into equivalence classes and provide an example of an input value for each class and determine the result for each case.

**Anwer_1 (boundary values):**
1. Age from 0 to 13 years old (inclusive):<br />
Output: "Impossible to issue", as persons under the age of 14 do not have the right to issue a passport.
2. Age from 14 to 115 years old (inclusive):<br />
Output: "Possible to issue", as persons aged 14 years and older have the right to issue a passport.
3. Age less than 0 or more than 115 years old:<br />
Output: "Error", since the input value is out of the acceptable range.

**Anwer_2 (equivalence classes):**
1. Any integer from 0 to 115 inclusive:<br />
Input: "0"<br />
Input: "13"<br />
Output: "Impossible to issue", as persons under the age of 14 do not have the right to issue a passport.<br />
Input: "14"<br />
Input: "115"<br />
Output: "Possible to issue", as persons aged 14 years and older have the right to issue a passport.

2. Any integer less than 0:<br />
Input: "-1"<br />
Output: "Error", since the input value is out of the acceptable range.

3. Any integer greater than 115:<br />
Input: "116"<br />
Output: "Error", since the input value is out of the acceptable range.

4. Non-integer inputs (Fractions, special characters, letters):<br />
Input: "14.5"<br />
Input: special character<br />
Input: letter<br />
Output: "Error", since the input value is not an integer.
