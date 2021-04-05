# WAD
This is a part of portolio for coursework

22.02.2021 - Development plan
---------------------------------------------------
public class Restaurant
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public string City { get; set; }
        public string Country { get; set; }
        public bool DineIn { get; set; }
        public CuisineType Cuisine { get; set; }
    }
public enum CuisineType
    {
        None = 0,
        Indian = 1,
        Chinese = 2,
        Mexican = 3
    }
---------------------------------------------------
public interface IRestaurantRepository
    {
        List<Restaurant> AllRestaurants();
        Restaurant GetRestaurantById(int id);
        Restaurant UpdateRestaurant(Restaurant updatedRestaurant);
        Restaurant CreateRestaurant(Restaurant newRestaurant);
        void DeleteRestaurant(int id);
    }public interface IRestaurantRepository
    {
        List<Restaurant> AllRestaurants();
        Restaurant GetRestaurantById(int id);
        Restaurant UpdateRestaurant(Restaurant updatedRestaurant);
        Restaurant CreateRestaurant(Restaurant newRestaurant);
        void DeleteRestaurant(int id);
    }
  -----------------------------------------------
  
