Download Link: https://assignmentchef.com/product/solved-cmsc204-assignment-1-passwords
<br>
Concepts tested by this program:

ArrayList

Tooltips

Mnemonic

Read  Files

Javadoc

JUnit Tests

Exceptions




Create an application that will check for valid passwords.  The following rules must be followed to create a valid password.




<ol>

 <li>At least 6 characters long</li>

 <li>10 or more characters is a strong password, between 6 and 9 characters is a weak (but acceptable) password.</li>

 <li>At least 1 numeric character</li>

 <li>At least 1 uppercase alphabetic character</li>

 <li>At least 1 lowercase alphabetic character</li>

 <li>No more than 2 of the same character in a sequence</li>

</ol>

Hello123 – OK

AAAbb123 – not OK

Aaabb123 – OK




<strong><u>Operation:</u></strong>

When the application begins, the user will be presented with a screen that states the above instructions for creating a password, two text entry boxes for typing in a password, and three buttons.

If the user wants to check a single password, they will type in the password in both boxes and select the “Check Password” button.

If the user wants to read in and check a list of passwords, they will select the “Check Passwords in File” button, be presented with a file explorer, and select the file to read from.  Those passwords that failed the check will be displayed, with their error message.

If the user presses the “Alt” key, a letter will be underlined in each button label.  That letter is the “mnemonic” that can used as a shortcut (Alt plus the letter) to execute the button.

If the user hovers his cursor over a button, a tooltip will be shown.

<strong><u>Specifications</u></strong>:




<strong>The Data Element</strong>

String

<strong>The Data Structure</strong>

ArrayList of Strings

<strong>Utility Class</strong>

Create a PasswordCheckerUtility class based on the Javadoc given you.  The PasswordCheckerUtility class will have at least three methods:  One method will check the validity of one password and return true if the password is valid and throw an exception if invalid.

One method will check for a “weak password”, i.e., one whose length is between 6 and 9, inclusive. Do NOT throw an exception.

One method will check an ArrayList of passwords and return an ArrayList with the status of any invalid passwords (weak passwords are not considered invalid).  The ArrayList of invalid passwords will be of the following format:

&lt;password&gt;&lt;space&gt;&lt;message of exception thrown&gt;

Create exception classes for each exception listed in PasswordCheckerUtility Javadoc.

Always check for the length of the password first, since that is the easiest and fastest check.  Once the password fails one rule, you do not need to check the rest of the rules.

<strong>The GUI</strong>

<ul>

 <li>Provide buttons to allow user to check validity of one password or a file of passwords.</li>

 <li>Ask the user to enter the password and to re-type the password. If the two are not the same, inform the user.</li>

 <li>Create a <u>tool tip</u> and a <u>mnemonic</u> for each of the buttons.</li>

 <li>Use a FileChooser for the user to select the input file.</li>

 <li>Use methods of PasswordCheckerUtility to process the passwords.</li>

 <li><u>Use try/catch structure to catch exceptions</u> thrown by PasswordCheckerUtility methods</li>

</ul>

<strong>Exceptions</strong>

<u>Provide exception classes</u> for the following:

<ol>

 <li>Length of password is less than 6 characters (class LengthException)</li>

</ol>

Message – The password must be at least 6 characters long

<ol start="2">

 <li>Password doesn’t contain an uppercase alpha character (class NoUpperAlphaException)</li>

</ol>

Message – The password must contain at least one uppercase alphabetic character

<ol start="3">

 <li>Password doesn’t contain a lowercase alpha character (class NoLowerAlphaException)</li>

</ol>

Message – The password must contain at least one lowercase alphabetic character

<ol start="4">

 <li>Password doesn’t contain a numeric character (class NoDigitException)</li>

</ol>

Message – The password must contain at least one digit

<ol start="5">

 <li>Password contains more than 2 of the same character in sequence (class InvalidSequenceException)</li>

</ol>

Message – The password cannot contain more than two of the same character in sequence.

<ol start="6">

 <li>For GUI – check if Password and re-typed Password are identical (class UnmatchedException)</li>

</ol>

Message – The passwords do not match

Throw this exception from the GUI, not the utility class.







If more than one error is present in a password, use the above order to throw exceptions.  For example, if a password is “xxyyzzwwaa”, it fails rules 2 and 4 above.  Throw a NoUpperAlphaException, not a NoDigitException.




<ul>

 <li>The file will be in the following format (one password per line):</li>

</ul>










Examples:




<ol>

 <li>No lowercase alphabetic character</li>

</ol>













Displayed to user:










<ol start="2">

 <li>No digit</li>

</ol>













Displayed to user:
















<ol start="3">

 <li>If the password is OK, but between 6 and 10 characters, you will see:</li>

</ol>




<ol start="4">

 <li>If password has more than two of the same characters in a row</li>

</ol>




Displayed to user:
















<ol start="5">

 <li>If password is valid</li>

</ol>







Displayed to user:










<ol start="6">

 <li>If the passwords do not match:</li>

</ol>










Displayed to user:










<ol start="6">

 <li>Based on the file above, when the user selects “Check Passwords in File”:</li>

</ol>




Displays errors to user when selecting Check Passwords in File. Note that valid passwords are NOT displayed.













<strong> </strong>

<u>Deliverables</u>:




<u>Design:</u>

<u> </u>

Initial design document (UML and pseudo-code)




<u>Implementation:</u>

Final design document INCLUDE JAVAFX

Java files – The src folder with your driver (javafx application), data manager, exceptions and Junit Test (.java) files

Javadoc files – The entire doc folder with your javadoc for student generated files

Learning Experience document

<em>single line comments</em>

<em>package declaration</em>

<em>GENERICS LAB</em>

<em>STUDY GUIDES?</em>

<u>Deliverable format</u>: The above deliverables will be packaged as follows. Two compressed files in the following formats:

LastNameFirstName_AssignmentX.zip [compressed file containing following]:

doc [a directory] <em>include the entire doc folder with the javadoc for </em>

<em>student generated files</em>

file1.html (example)

file2.html (example)

class-use (example directory)

LearningExperience.doc <em>or other text format</em>

src [a directory] <em>contains your driver (javafx application), data manager, exceptions and Junit Test (.java) files</em>

File1.java (example)

File2.java (example)

File_Test.java (example)

LastNameFirstName_AssignmentX_<strong>Moss</strong>.zip [compressed file containing only]:

<em>.java file which includes the driver (javafx application), data manager, exceptions and Junit Test (.java) files – </em><em>NO </em>

<em>FOLDERS!!</em>

File1.java (example)

File2.java (example)

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong>Grading Rubric</strong>

<strong>CMSC 204 Project #1</strong>

Name _____________________________




<strong><u>Overview</u></strong><strong>: </strong>

There are two parts to the rubric.   First, the project is graded on whether it passes public and private tests.  If it does not compile, a 0 will be given. These points add up to 100.  Second, the score is decremented if various requirements are not met, e.g., no Javadoc, no UML diagram, uses constructs that are not allowed, etc.




<strong><u>TESTING</u></strong><strong>        </strong>(100 pts)<strong>          </strong><strong>                                                </strong>

Passes Public JUnit tests without runtime exceptions thrown on console   20 pts _____

Passes JUnit student tests                                                                               5 pts _____

Passes private instructor tests                                                                       75 pts _____

Possible Sub-total                                                                               100 pts _____

<strong><u>REQUIREMENTS</u></strong>  (Subtracts from Testing total)

<strong><u>Documentation:</u></strong>

Javadoc for student generated files not submitted (entire doc folder)        -6 pts _____

Documentation within source code was missing or incorrect                     -6 pts _____

Description of what class does was missing

Author’s Name, @author, was missing

Methods not commented properly using Javadoc @param, @return

JUnit STUDENT methods were not implemented                                      -6 pts _____

Learning Experience                                                                                    -4 pts _____

In 3+ paragraphs, highlight your lessons learned and learning experience from working on this project.  What have you learned? What did you struggle with? What would you do differently on your next project?

<strong><u>Programming Style:</u></strong>

Incorrect use of indentation, statements, structures                                     -8 pts _____

User Interface                                                                                              -6 pts _____

Not clear to user how data is to be entered; UI does not follow requirements

Output is not easy to understand

<strong><u>Design:</u></strong>

Classes do not have the functionality specified, i.e.,

<ol>

 <li>PasswordCheckerUtility class                                                          -8 pts _____</li>

</ol>

does not have a method to check validity of password

does not have a method to check validity of  ArrayList of passwords

does not follow the Javadoc provided

<ol start="2">

 <li>GUI                         -8 pts _____</li>

</ol>

does not use methods of PasswordCheckerUtility

does not display status of password entered by user

buttons do not have tooltips and mnemonics

<ol start="3">

 <li>Exceptions classes                                                                         -8 pts _____</li>

</ol>

does not have exception class for each invalid password rule

does not have exception class if password and re-type password don’t match

Possible decrements:                                                                          -60 pts _____

Possible total grade:                                                                             100 pts _____