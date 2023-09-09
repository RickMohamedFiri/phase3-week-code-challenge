# Restaurants without sqlalchemy

This is a simple Python implementation of a Restaurant Review System, comprising three main classes: `Customer`, `Restaurant`, and `Review`. These classes are designed to handle customer data, restaurant data, and reviews respectively.


### Methods

- `__init__(given_name, family_name)`: Initializes a customer with a given name and family name.
- `given_name()`: Returns the customer's given name.
- `family_name()`: Returns the customer's family name.
- `full_name()`: Returns the full name of the customer.
- `all()`: Returns a list of all customer instances.
- `add_review(restaurant, rating)`: Adds a review for a specific restaurant with a given rating.
- `restaurants()`: Returns a list of unique restaurants reviewed by the customer.
- `num_reviews()`: Returns the total number of reviews the customer has authored.
- `find_by_name(name)`: Returns the first customer whose full name matches the provided name.
- `find_all_by_given_name(name)`: Returns a list of customers with the given name.

## Restaurant Class

### Methods

- `__init__(name)`: Initializes a restaurant with a name.
- `name()`: Returns the restaurant's name.
- `all()`: Returns a list of all restaurant instances.
- `add_review(review)`: Adds a review to the restaurant's list of reviews.
- `reviews()`: Returns a list of reviews for the restaurant.
- `customers()`: Returns a unique list of customers who have reviewed the restaurant.
- `average_star_rating()`: Calculates and returns the average star rating for the restaurant based on its reviews.

## Review Class

### Methods

- `__init__(customer, restaurant, rating)`: Initializes a review with a customer, restaurant, and rating.
- `rating()`: Returns the rating for the review.
- `all()`: Returns a list of all review instances.
- `customer()`: Returns the customer object associated with the review.
- `restaurant()`: Returns the restaurant object associated with the review.

## Usage

1. Create instances of customers, restaurants, and reviews.
2. Interact with customer and restaurant instances using the provided methods.
3. Obtain information about reviews and relationships between customers and restaurants.

## Example

```python
# Creating instances
customer1 = Customer("John", "Doe")
restaurant1 = Restaurant("Bistro Delight")

# Adding a review
customer1.add_review(restaurant1, 4)

# Getting customer's reviewed restaurants
reviewed_restaurants = customer1.restaurants()

# Getting restaurant's average star rating
average_rating = restaurant1.average_star_rating()

```


# License
This project is licensed under the MIT License.
Author Rick Mohamed
