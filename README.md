1. Project Elevator Pitch
    A website/app for users to rent/loan seasonal outdoor equipment for vacations when an owner might not be using it, such as beach chairs/umbrellas, hiking equipment, climbing equipment, ski equipment, surfboards, kayaks and other watersport equipment. Its AirBnb for outdoors activity goods.

2. Database Schema
    See DBSchema.png file.

3. List of API Endpoints
        /users router

            POST /users/register
 
            POST /users/login
        
            🔒 GET /users/me
            Returns the currently logged-in user's data, rentals, and listings
        
        /products router

            GET /products 

            GET /products/:id

            🔒 GET /products/:user 
            shows a users current listed products
        
            GET /products/:id/reviews
        
            🔒 POST /products/:id/reviews

        /rentals router

            🔒 POST /rentals
  
            🔒 GET /rentals
            sends array of all rentals made by the logged-in user

            🔒 GET /rentals/:id
  
4. Front end Wireframe
    See Wireframe.png file

5. User story
    Unathenticated users will be able to view products available to rent and view reviews for items, but won't be able to rent items, list items for rent, submit reviews, or see account details.
    Authenticated users can rent items, list items, submit reviews, and see account details.