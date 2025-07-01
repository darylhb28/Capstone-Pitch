1. Project Elevator Pitch
    A website/app for users to rent/loan seasonal outdoor equipment for vacations when an owner might not be using it, such as beach chairs/umbrellas, hiking equipment, climbing equipment, ski equipment, surfboards, kayaks and other watersport equipment. Its AirBnb for outdoors activity goods.

2. Database Schema

    https://dbdiagram.io/d/Nomad-DB-6861665bf413ba350865b708

3. List of API Endpoints
        /users router

            POST /users/register
 
            POST /users/login
        
            🔒 GET /users/me
            Returns the currently logged-in user's data, rentals, listings, and messages
        
        /products router

            GET /products 

            GET /products/:id

            🔒 GET /products/:user_id
            shows a users current listed products

        /rentals router

            🔒 POST /rentals
  
            🔒 GET /rentals
            sends array of all rentals made by the logged-in user

            🔒 GET /rentals/:id

            🔒 GET /rentals/:user_id
            shows a users current rented products

        /messages router

            🔒 POST /messages
  
            🔒 GET /messages

            🔒 GET /messages/:id

            
  
4. Front end Wireframe
    See Wireframe.png file

5. User story
    Unathenticated users will be able to view products available to rent, but won't be able to rent items, list items for rent, send messages, or see account details.
    Authenticated users can rent items, list items, send messages, and see account details.