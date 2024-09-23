# Coffee Shop Domain Modeling

# Overview
The Coffee Shop project is a simple implementation of a coffee shop management system using Python classes. It includes classes for Customer, Coffee and Order, each with methods for defining object relationships and implementing aggregate and association methods.

# Table of content
  - [Installation](#installation)
  - [Usage](#usage)
  - [Code Structure](#code-structure)
  - [***customer.py***](#customerpy)
  - [***coffee.py***](#coffeepy)
  - [***order.py***](#orderpy)
  - [Contributing](#contributing)
  - [License](#license)

## Installation
To run this project, you need to have Python installed on your system. You can download Python from the official website: https://www.python.org/downloads/

### Usage
To use this project, follow these steps:

1. Clone or fork the project from the GitHub repository: https://github.com/NzauM/coffee-shop to your local machine.
    
2. In your IDE terminal(VSCode) navigate to the project directory.
    ```
    cd coffee-shop
    ```
3. Install a virtual environment for this project
    ```
    pipenv install
    ```
4. Open a subshell
    ```
    pipenv shell
    ```
5. ***Runfile.py*** runs the code for the customer, coffee and order classes.
   To execute the code examples in  ***Runfile.py*** run this command in the terminal:
     ```
     python runfile.py
     ```

## Code Structure
The project has been organized to 3 files for each class: ***customer.py***, ***coffee.py***, and ***order.py***. Each file contains the definition of the respective class and its methods.

The code will be run from the : ***runfile.py***as is outlined in the [Usage](#usage) section.

  ### ***customer.py***
The ***customer.py*** file defines the Customer class, which represents a customer in the coffee shop. The class provides the following functionality:

   - *Initialization:* Creates a Customer instance with a name.
   - *Order Creation:* Allows a customer to create new orders for different coffees, which are then associated with this customer.
   - *Order Retrieval:* Provides a method to retrieve all orders associated with the customer.
   - *Coffee Retrieval:* Provides a method to retrieve a list of all coffee types that the customer has ordered.

  ### ***coffee.py***
The ***coffee.py*** file defines the Coffee class, which represents a type of coffee available in the coffee shop. The class provides the following functionality:
  - *Initialization:* Creates a Coffee instance with a name.
  - *Order Retrieval:* Provides a method to retrieve all orders associated with a given Coffee instance.
  - *Customer Retrieval:* Provides a method to retrieve all unique customers who have ordered a given Coffee instance.
  - *Order Count:* Provides a class method to count the total number of orders for a specific Coffee instance.
  - *Average Price:* Provides a class method to calculate the average price of orders for a specific Coffee instance.

### ***order.py***
The ***order.py*** file defines the Order class, which represents an order placed by a customer for a specific type of coffee. The class provides the following functionality:

 - *Initialization:* Creates an Order instance with a Customer and a Coffee instance and a price. 
 -  Each property(customer, coffee, price) is created with a getter and setter method that offers validation.
 -  It also updates the orders associated with the customer and the coffee.

## Contributing
If you would like to contribute to this project, please follow these steps:

1. Fork the repository on GitHub: [https://github.com/NzauM/coffee-shop](repository)
2. Create a new branch for your changes: git checkout -b your-feature-branch
3. Make your changes and commit them: git commit -am 'Add your feature'
4. Push your changes to your fork: git push origin your-feature-branch
5. Create a pull request on GitHub to merge your changes into the main repository.

## License
This project is licensed under the MIT License. See the [https://github.com/NzauM/LICENCE](LICENCE) file for more details.
