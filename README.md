# Customer, Restaurant, and Review Management System

This Python code demonstrates a simple management system for customers, restaurants, and reviews. It allows you to create customers, restaurants, and reviews, and retrieve information about them.

# Table of Contents

- [Overview](#overview)
- [Usage](#usage)
- [Classes](#classes)
- [Example](#example)

## Overview

The code provides three classes:
- Customer: Represents a customer with given name, family name, and reviews.
- Restaurant: Represents a restaurant with a name, reviews, and associated customers.
- Review: Represents a review with a customer, restaurant, and rating.

The code shows how to create instances of customers, restaurants, and reviews, and retrieve information from them.

## Usage

1. Clone the repository to your local machine.

2. Open the Python file (main.py) in your preferred Python environment.

3. Run the Python file to see the example in action. It demonstrates how to create customers, restaurants, and reviews, and retrieve their information.

## Classes

### Customer

Represents a customer with given name, family name, and reviews.

Methods:
- get_given_name(): Get the customer's given name.
- get_family_name(): Get the customer's family name.
- full_name(): Get the customer's full name.

### Restaurant

Represents a restaurant with a name, reviews, and associated customers.

Methods:
- get_name(): Get the restaurant's name.
- get_reviews(): Get the reviews associated with the restaurant.
- get_customers(): Get the customers who have reviewed the restaurant.

### Review

Represents a review with a customer, restaurant, and rating.

Methods:
- get_rating(): Get the review's rating.
- customer(): Get the associated customer.
- restaurant(): Get the associated restaurant.

## Example

Here's an example of how to use the code:

    python
# Create an instance of Customer for customer1
customer1 = Customer("Joyce", "Wachira")

# Create an instance of Restaurant for restaurant1
restaurant1 = Restaurant("Gourmet Foods and Drinks")

# Adding a review
my_review = Review(customer1, restaurant1, 70)

# Retrieving your review's rating and associated customer and restaurant
print(f"My review rating: {my_review.get_rating()}")
print(f"Customer: {my_review.customer().full_name()}")
print(f"Restaurant: {my_review.restaurant().get_name()}")
