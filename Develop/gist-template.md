Title:Tutorial to Regex for email address

Regex, or regular expressions, are and sequence of characters which can define and validate a specific pattern. Regular expressions can be a combination of letters, numbers, special characters, and quantifiers.

Summary
Today i will be covering and breaking down the compenents of regular expressions that are used to validate an email address. This is the regex code that we will analyze today: /^w+[+.w-]*@([w-]+.)*w+[w-]*.([a-z]{2,4}|d+)$/i

Table of Contents
Anchors
Quantifiers
Character Classes
Grouping and Capturing
Bracket Expressions
Greedy and Lazy Match
Regex Components
Anchors
The anchors that we use to contain this particular Regex are ^ to start and $ to finish.

Quantifiers
In our example regex we used + a few times in our expression. This is an example of a greedy quantifier. We also used {2,4} towards the end of the expression, this is another greedy quantifier that specifies the input needs to be a minimum of 2 characters but no more than 4 characters.

Character Classes
In our regex, the character class \w is used. Jacascript classifies this as a use of any word (letters, digits, underscores).

Grouping and Capturing
There are three groups being captured in out example. The first is: /^w+[+.w-]*@. This is the "user name" and it captures everything before the @. The second group is: ([w-]+.)*w+[w-]*.. This is the "domain name" and it captures everything in between the @ and the .. The third and final group: ([a-z]{2,4}|d+)$/i captures the "extension", or everything that comes after the .. (i.e .com or .net)

Bracket Expressions
We have four different bracket expressions in out example expression! The information inside of the bracket is held in open/close bracketsm like this []. This identifies which information is matched.

Greedy and Lazy Match
In our example we only have greedy matches, + and {}. This means that it will allow the match to expand as long s it needs to. If we were to have used lazy quantifiers, then they would look like +? and {}?. These would direct the system to make the shortest match it can.

Author
My name is Yizhong Wang , There is my github link https://github.com/YizhongWang
