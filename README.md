# Continental.js
A JavaScript object with information about all countries of the world. Information includes population, surface area, languages and much more.

Every country is an additional object attached to the countries object. They include 10 properties, which might be useful when trying to extract information for a project.

Example object:
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

The ten properties are as follows:
- Name
- PopulationN (in Numbers e.g. 34566713)
- PopulationW (in Words e.g. "34.56M")
- Surface Area
- Map (flag map in .png)
- Capital City
- Languages (Always in an array)
- Predominent Religion
- Cities (An array of the 3 most populated cities, in order)
- Dish (National Dish in a string)
- 
