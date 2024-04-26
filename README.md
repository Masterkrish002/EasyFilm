# EasyFilm
EasyFilm is an innovative website dedicated to providing users with comprehensive information about movies. Designed to be user-friendly and feature rich, EasyFilm offers a dynamic platform for accessing details about various films. Built on the .NET framework, EasyFilm is committed to delivering a seamless browsing experience, empowering users to explore movie details effortlessly.
# How to run it
1. clone the project
   `git clone https://github.com/Masterkrish002/EasyFilm`
2. open `appsettings.json` file and update connection string's `data source=your server name`
   
   ``` 
    "ConnectionStrings": {
          "conn": "data source=your_server_name;initial catalog=MovieStoreMvc; integrated security=true;encrypt=false"
     }
   ```

3. Delete `Migrations` folder
4. Open Tools > Package Manager > Package manager console
5. Run these 2 commands
    ```
     (i) add-migration init
     (ii) update-database
     ````
7. Now you can run this project

## How to Register as a admin and login?
1. There is a controller `UserAuthentication` and a commented method `Register`. Uncomment the `Register` method
2. Run the project and hit the url `https://localhost:7095/UserAuthentication/Register`. You will be registered as a admin. Now you can re comment the register user (for privacy).
3. Now you can login with credentials `Username: admin, password: Admin@123`

