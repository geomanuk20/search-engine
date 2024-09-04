# search-engine

#HTML


Search Form: The form contains an input field where users can type their search query.
The onkeyup event triggers the search() function every time a key is released, allowing for real-time filtering.

Product List: The products are displayed within the div with the class product-list. 
Each product is wrapped in a div with the class product. Inside each product div, there's an image and product details like the name and price.

Font Awesome Icon: The search icon (magnifying glass) is added using Font Awesome for better visual representation.

#js

Search Box Value: The function starts by getting the value of the search box,
converting it to uppercase (.toUpperCase()) to ensure the search is case-insensitive.

Product Elements:

storeitems refers to the product-list div that contains all the products.
products is a NodeList of all elements with the class product.
pname(productname) is a collection of all the h5 elements inside the product-list, representing the product names.

Loop through Products:

The for loop iterates over each product. For each product, it checks if the product name (h5 element) contains the search term.
match gets the h5 element inside the current product.

Check for Match:

The textvalue variable holds the product name's text content.
The indexOf(searchbox) method checks if the search term exists within the product name (textvalue). If it does, the index will be greater than -1, indicating a match.

Display or Hide Products:

If a match is found, the product remains visible (products[i].style.display = "").
If there's no match, the product is hidden (products[i].style.display = "none").
