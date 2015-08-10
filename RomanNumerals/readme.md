Learn the Romans Number for the Glory of Rome!!
======================================

The Romans were a clever bunch. They conquered most of Europe and ruled it for hundreds of years. They invented concrete and straight roads and even bikinis. 
One thing they never discovered though was the number zero. This made writing and dating extensive histories of their exploits slightly more challenging, but the system of numbers they came up with is still in use today. For example the BBC uses Roman numerals to date their programmes.

The Romans wrote numbers using letters - I, V, X, L, C, D, M. (notice these letters have lots of straight lines and are hence easy to hack into stone tablets)

For a full description of how it works, take a look at [ http://www.novaroma.org/via_romana/numbers.html ]: which includes an implementation of the Kata in javascript.

There is no need to be able to convert numbers larger than about 3000. (The Romans themselves didn't tend to go any higher)

*Note that you can't write numerals like "IM" for 999. Wikipedia says: Modern Roman numerals ... are written by expressing each digit separately starting with the left most digit and skipping any digit with a value of zero. To see this in practice, consider the ... example of 1990. In Roman numerals 1990 is rendered: 1000=M, 900=CM, 90=XC; resulting in MCMXC. 2008 is written as 2000=MM, 8=VIII; or MMVIII.*

Part I
===================
As a user
	Given a decimal number
	I want to convert it to the Roman numerals

<pre>
*     1 --> I
*     10 --> X
*     7 --> VII
*     3146 -> MMMCXLVI
</pre>

Part II
===================
As a user
	Given a Roman numeral
	I want to convert it to the decimal form
	
<pre>
* III -> 3
* XXXII -> 32
* CXXIII -> 123
* MMMCCCXXXIII -> 3333
</pre>


Part III
===================
You are the imperial accontant of Cesare, the glorious emperatour. And you have to count the taxes that each farmer has to paid to Cesare. 
The cost is 2 Sestertius for each square foot of land, the imperial unit of area.
As accountance of the emperator you have to parse a textual file with the following format:
	
As the imperial accountant
	Given the "List of Lands"
	I want to produce the "List of Taxes" to be paid to Cesare
	
		
**Input Received**
<pre>
	## LIST OF LANDS ##
	
	>> Agostino Piedone
	IV x III ft
	V x VII ft
	VIII x V ft
	
	>> Mario della Romina
	IV x IV ft
	VI x II ft
	
	>> Pino Saluto
	III x IV ft
	V x VII ft
</pre>
	
**Output to produce**
<pre>
	## LIST OF TAXES ##

	Agostino Piedone:
	- habet reddere CLXXIV Sestertius
	
	Mario della Romina:
	- habet reddere LVI Sestertius
	 
	Pino Saluto: 
	- habet reddere CMIV Sestertius
</pre>

