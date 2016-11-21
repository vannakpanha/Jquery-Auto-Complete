# Auto-complete Jquery Ajax

## Usage
- Add all the javascript and css file into you source code
- Write the following script
 
$('.autocomplete').autocomplete({
	serviceUrl: 'http://localhost:8000/en/booking/search_customer',
	paramName: 'name',
	onSelect: function (suggestion) {
		console.log(suggestion);
	}
});

- paramName is a variable that going to use for query in you controller
- onSelect is the function process when we select any item 

## Response 
- Make sure you respon from request follow the fomate like bellow 

{"suggestions":[{"value":"Sothea Su","data":1},{"value":"Chanvotey Cheng","data":2}]}
