---
title: "Expressions"
url: /refguide7/expressions/
parent: "common-elements"
aliases:
    - /refguide7/microflow-expressions.html
description: "Describes the expressions that can be used in Mendix for a variety of purposes (for example, to change a member of an object based on logic)."
#If moving or renaming this doc file, implement a temporary redirect and let the respective team know they should update the URL in the product. See Mapping to Products for more details.
---

Expressions can for example be used to change a member of an object based on logic. Variables in the microflow can be called in an expression by inserting the name of the variable and adding a dollar sign. E.g. _$customer_ refers to the variable _customer_. Expressions can be used recursively, for example, _1 + 2 + 3_. Attributes and associations of object variables are accessed using a slash, for example, _$customer/Name_, _$customer/CRM.Customer_Order_.

To illustrate this imagine an object with variable name _package_ with two attributes: _weight_ (Float) and _shippingCosts _(Decimal). Rule: if the weight of a package is less than one kilogram there are no shipping costs. Otherwise the shipping costs are €5.00\. The expression for changing attribute _shippingCosts_ is: _if $package/weight < 1.00 then 0.00 else 5.00_.

An overview of the possibilities with expressions can be found below.

### [Unary Expressions](/refguide/unary-expressions/):

* [Unary minus ( - )](/refguide/unary-expressions/)

### [Arithmetic Expressions](/refguide/arithmetic-expressions/):

* [Multiplication ( * )](/refguide/arithmetic-expressions/)
* [Division ( div or : )](/refguide/arithmetic-expressions/)
* [Modulo ( mod )](/refguide/arithmetic-expressions/)
* [Addition ( + )](/refguide/arithmetic-expressions/)
* [Subtraction ( - )](/refguide/arithmetic-expressions/)

### [Relational Expressions](/refguide/relational-expressions/):

* [Less than ( < )](/refguide/relational-expressions/)
* [Greater than ( > )](/refguide/relational-expressions/)
* [Less than or equal to ( <= )](/refguide/relational-expressions/)
* [Greater than or equal to ( >= )](/refguide/relational-expressions/)
* [Is equal to ( = )](/refguide/relational-expressions/)
* [Is not equal to ( != )](/refguide/relational-expressions/)

### [Special checks](/refguide/special-checks/)

* [Checking for an empty object](/refguide/special-checks/)
* [Checking for an empty object member](/refguide/special-checks/)
* [`isNew`](/refguide/special-checks/) - Checking whether an object is new

### [Boolean expressions](/refguide/boolean-expressions/)

* [and](/refguide/boolean-expressions/)
* [or](/refguide/boolean-expressions/)
* [not](/refguide/boolean-expressions/)

### [If expressions](/refguide/if-expressions/)

### [Mathematical function calls](/refguide/mathematical-function-calls/)

* [`max`](/refguide/mathematical-function-calls/) - Maximum of a list of numbers
* [`min`](/refguide/mathematical-function-calls/) - Minimum of a list of numbers
* [`round`](/refguide/mathematical-function-calls/) - Rounding a floating-point number, optionally to a specified precision
* [`random`](/refguide/mathematical-function-calls/) - Random number generation
* [`floor`](/refguide/mathematical-function-calls/) - Rounding a floating-point number down
* [`ceil`](/refguide/mathematical-function-calls/) - Rounding a floating-point number up
* [`pow`](/refguide/mathematical-function-calls/) - Exponentiation
* [`abs`](/refguide/mathematical-function-calls/) - Absolute value
* [`floatsEqual` `/ currenciesEqual`](/refguide/mathematical-function-calls/) - Equality of floats/currencies for a certain precision (deprecated)

### [String function calls](/refguide/string-function-calls/)

* [`toUpperCase`](/refguide/string-function-calls/) - Convert string to uppercase
* [`toLowerCase`](/refguide/string-function-calls/) - Convert string to lowercase
* [`length`](/refguide/string-function-calls/) - String length
* [`substring`](/refguide/string-function-calls/) - Get part of a string
* [`find`](/refguide/string-function-calls/) - Get substring position
* [`findLast`](/refguide/string-function-calls/) - Get last substring position
* [`contains`](/refguide/string-function-calls/) - Contains substring
* [`startsWith`](/refguide/string-function-calls/)  - Determine whether a string starts with the specified substring
* [`endsWith`](/refguide/string-function-calls/)  - Determine whether a string ends with the specified substring
* [`trim`](/refguide/string-function-calls/) - Remove leading and trailing whitespace
* [`isMatch`](/refguide/string-function-calls/) - Match regular expression
* [`replaceAll`](/refguide/string-function-calls/) - Replace occurrences of substring
* [`replaceFirst`](/refguide/string-function-calls/) - Replace first occurrence of substring
* [String concatenation ( + )](/refguide/string-function-calls/) - Concatenate strings
* [`urlEncode`](/refguide/string-function-calls/) - Convert a string to be used in a URL
* [`urlDecode`](/refguide/string-function-calls/) - Convert a string back from a URL

### [Date creation](/refguide/date-creation/)

* [`dateTime`](/refguide/date-creation/) - Creating a date value using the server's calendar
* [`dateTimeUTC`](/refguide/date-creation/) - Creating a date value using the UTC calendar

### [Between date function calls](/refguide/between-date-function-calls/)

* [`millisecondsBetween`](/refguide/between-date-function-calls/) - Milliseconds between two dates
* [`secondsBetween`](/refguide/between-date-function-calls/) - Seconds between two dates
* [`minutesBetween`](/refguide/between-date-function-calls/) - Minutes between two dates
* [`hoursBetween`](/refguide/between-date-function-calls/) - Hours between two dates
* [`daysBetween`](/refguide/between-date-function-calls/) - Days between two dates
* [`weeksBetween`](/refguide/between-date-function-calls/) - Weeks between two dates

### [Add date function calls](/refguide/add-date-function-calls/)

* [`addMilliseconds`](/refguide/add-date-function-calls/) - Add milliseconds to a date
* [`addSeconds`](/refguide/add-date-function-calls/) - Add seconds to a date
* [`addMinutes`](/refguide/add-date-function-calls/) - Add minutes to a date
* [`addHours`](/refguide/add-date-function-calls/) - Add hours to a date
* [`addDays`](/refguide/add-date-function-calls/) - Add days to a date
* [`addDaysUTC`](/refguide/add-date-function-calls/) - Add days to a date using the UTC calendar
* [`addWeeks`](/refguide/add-date-function-calls/) - Add weeks to a date
* [`addWeeksUTC`](/refguide/add-date-function-calls/) - Add weeks to a date using the UTC calendar
* [`addMonths`](/refguide/add-date-function-calls/) - Add months to a date
* [`addMonthsUTC`](/refguide/add-date-function-calls/) - Add months to a date using the UTC calendar
* [`addYears`](/refguide/add-date-function-calls/) - Add years to a date
* [`addYearsUTC`](/refguide/add-date-function-calls/) - Add years to a date using the UTC calendar

### [Trim to date](/refguide/trim-to-date/)

* [`trimToSeconds`](/refguide/trim-to-date/) - Trim to seconds
* [`trimToMinutes`](/refguide/trim-to-date/) - Trim to minutes
* [`trimToHours`](/refguide/trim-to-date/) - Trim to hours
* [`trimToHoursUTC`](/refguide/trim-to-date/) - Trim to hours using the UTC calendar
* [`trimToDays`](/refguide/trim-to-date/) - Trim to days
* [`trimToDaysUTC`](/refguide/trim-to-date/) - Trim to days using the UTC calendar
* [`trimToMonths`](/refguide/trim-to-date/) - Trim to months
* [`trimToMonthsUTC`](/refguide/trim-to-date/) - Trim to months using the UTC calendar
* [`trimToYears`](/refguide/trim-to-date/) - Trim to years
* [`trimToYearsUTC`](/refguide/trim-to-date/) - Trim to years using the UTC calendar

### [To string](/refguide/to-string/)

### [To float](/refguide7/to-float/) (deprecated)

### [Parse integer](/refguide/parse-integer/)

### [Parse/format float function calls](/refguide7/parse-and-format-float-function-calls/) (deprecated)

* [`parseFloat`](/refguide7/parse-and-format-float-function-calls/) - Convert a string to a float
* [`formatFloat`](/refguide7/parse-and-format-float-function-calls/) - Convert a float to a string

### [Parse/format decimal function calls](/refguide/parse-and-format-decimal-function-calls/)

* [`parseDecimal`](/refguide/parse-and-format-decimal-function-calls/)  - Convert a string to a decimal
* [`formatDecimal`](/refguide/parse-and-format-decimal-function-calls/)  - Convert a decimal to a string

### [Parse/format date function calls](/refguide/parse-and-format-date-function-calls/)

* [`parseDateTime[UTC]`](/refguide/parse-and-format-date-function-calls/) - Convert a string to a date value
* [`formatDateTime[UTC]`](/refguide/parse-and-format-date-function-calls/) - Convert a date value to a string
* [`formatTime[UTC]`](/refguide/parse-and-format-date-function-calls/) - Convert the time part of a date value to a string
* [`formatDate[UTC]`](/refguide/parse-and-format-date-function-calls/) - Convert the date part of a date value to a string

### [Enumerations in expressions](/refguide/enumerations-in-expressions/)

* [`getCaption`](/refguide/enumerations-in-expressions/) - Get caption of enumeration value in current language
* [`getKey`](/refguide/enumerations-in-expressions/) - Get technical name of enumeration value
