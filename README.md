# Continental.js
A JavaScript **object** with information about _all_ countries of the world. Information includes population, surface area, languages and much more 😉.
> To see full list, find [**"Properties"**](##-properties) section below.

## Add to HTML 
Paste the following code into your `<head>` or the beginning of `<body>` in your `HTML` file:
```html
<script src="https://c.jalalprohacker.repl.co/continental.js"></script>
```
> The code is stored in Replit. [See full code](https://c.jalalprohacker.repl.co/continental.js)

# Contents
- [**Properties**](#-properties)
- [**Examples**](#-examples)
- [**Notes**](#-notes)

## Properties
Below are the ten properties that the code provides:
#### Name
Provided in a string.
```javascript
console.log(continental.countries.afghanistan.name); // Returns "Afghanistan"
```
#### Population (Numbers)
Provides population number in an integer
```javascript
console.log(continental.countries.afghanistan.populationN); // Returns 41984070
```
#### Population (Words)
Provides population number in a string, including an `integer` followed by abbreviation `(K/M/B)`
```javascript
console.log(continental.countries.afghanistan.populationW); // Returns "41.98M"
```
#### Surface Area (km2)
Provides surface area in `string` format
```javascript
console.log(continental.countries.afghanistan.area); // Returns "652,860 km²"
```
#### Flag Map (.png)
Returns flag map **URL** in `.png` format
```javascript
console.log(continental.countries.afghanistan.map); // Returns "https://upload.wikimedia.org/wikipedia/commons/b/bc/Flag_map_of_Afghanistan.png"
```
#### Capital City
Returns capital city name in `string`
```javascript
console.log(continental.countries.afghanistan.capital); // Returns "Kabul"
```
#### Languages
Returns **array** with languages of country
_There will still be an array if there is one language. For best results, use `languages[0]`._
```javascript
console.log(continental.countries.afghanistan.languages[0]); // Returns "Dari"
console.log(continental.countries.afghanistan.languages[1]); // Returns "Pashto"
```
#### Religion
Returns predominent religion of country in a `string`.
```javascript
console.log(continental.countries.afghanistan.religion); // Returns "Islam"
```
#### Big Cities
Returns **array** with **three** most populated cities of country, _in order_.
```javascript
console.log(continental.countries.afghanistan.cities[0]); // Returns "Kabul"
console.log(continental.countries.afghanistan.cities[1]); // Returns "Kandahar"
console.log(continental.countries.afghanistan.cities[2]); // Returns "Herat"
```
#### National Dish
Returns national dish of country as `string`.
```javascript
console.log(continental.countries.afghanistan.dish); // Returns "Kabuli"
```
## Examples
**Full object for Afghanistan:**
```javascript
afghanistan: {
	name: "Afghanistan",
	populationN: 41984070,
	populationW: "41.98M",
	area: "652,860 km²",
	map: "https://upload.wikimedia.org/wikipedia/commons/b/bc/Flag_map_of_Afghanistan.png",
	capital: "Kabul",
	languages: ["Dari", "Pashto"],
	religion: "Islam",
	cities: ["Kabul", "Kandahar", "Herat"],
	dish: "Kabuli",
}
```
**Comparing populations of Afghanistan and Argentina:**
```javascript
var x = continental.countries.afghanistan.populationN;
var y = continental.countries.argentina.populationN;
if(x > y){
	console.log("Afghanistan has a higher population.");
} else if(y > x){
	console.log("Argentina has a higher population.");
}
```
**Asking questions about countries:**
```javascript
var x = prompt("What is Afghanistan's national dish?");
var y = continental.countries;
if(x.toLowerCase() === y.afghanistan.dish.toLowerCase()){
	alert("You are correct!");
} else{
	alert("Incorrect. The correct answer is " + y.afghanistan.dish);
}
```
## Notes
- The code is all hand-written, so if you find anything wrong, please let me know :)
- While storing code in `Replit` is unusual, it doesn't have any weaknesses.
- Share your feedback and suggestions, I would love to hear them.

_Made with ❤️ from London_
