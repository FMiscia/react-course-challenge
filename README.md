## React Course Challenge
Create a React app that allows users to Login, view a list of products and save the product they like on a personal page.

**Requirements**:

 - **Create 3 different pages**
	 - Login page
	 - Products page
	 - Profile page
 - **Login page**:
	 -	
	 - Create a simple form with email and password inputs
	 - The **login api** is a POST request to: https://api.escuelajs.co/api/v1/auth/login and accepts a json object like the following: 
	` { "email": "john@mail.com", "password": "changeme" }`
 - **Products page**
	 -	
	 - Show a list of products using the following API GET: https://api.escuelajs.co/api/v1/products/
	 - Every product should show at least the **title**,  the **image** (just one),  the **price** and the **description** of the product (all this data are available from the API)
	 - Every product should have a button to save it to the favourite products and, if the products is already saved, the button should remove the element from the saved ones (no api here just save the elements on the client side)
	 - The list can be alphabetically ordered on the title
 - **Profile page**
	 - 
	 - Show the profile information from the following API GET: https://api.escuelajs.co/api/v1/auth/profile/
	 - Show the list of saved products with the possibility to remove the elements.

IMPORTANT DETAILS:
- 
- The LOGIN api returns an **access_token**. It has to be used as "Bearer" token, so the other requests should have the following header `"Authorization": "Bearer ${access_token}"`
- The Products Page and the Profile Page **should not be accessible** if the user isn't logged in
- **The profile api** is the only authenticated request, so you can **use that API to check if the user is logged in or not** when the app is refreshed (so, **save the access_token somewhere**).
- Does not matter if  the saved products are lost after a refresh don't spend time to serialize that information.
- You can use **every library you want** and **even reuse the components we created during the course**
