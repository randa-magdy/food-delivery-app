# Food Delivery Application

## Content List

1. [Vision](#vision)
2. [Features and Functionalities for the System](#features-and-functionalities)
3. [Use Case Model for the System](#use-case-model-for-the-system)  
   3.1. [Actors](#actors)  
   3.2. [Use Cases](#use-cases)  
   3.3. [Use Case Diagram](#use-case-diagram)
---

## Vision  

The food delivery application is designed to offer customers a smooth and intuitive experience for discovering and ordering meals. Users can effortlessly search for nearby restaurants, explore menus with ease, and place orders quickly and without complications. The app also enables customers to track and manage their orders, take advantage of special discounts and promotions, and enjoy reliable, timely deliveries tailored to their schedules.

---

## Features and Functionalities for the System 

The detailed list of system features and functionalities is available in a separate document.  
Please refer to [Features and Functionalities Document](./features-documentation.md) for more details.

---

## Use Case Model for the System 

### `Actors of the System` 
- **Customer** : Searches for restaurants, browses menus, places orders, makes payments, and tracks deliveries.  
- **Restaurant Owner/Manager** : Manages restaurant listings, updates menus, processes orders, and handles order statuses.  
- **Restaurant/Kitchen Staff** : Prepares the food once an order is received.  
- **Delivery Person (Driver)** : Picks up orders from restaurants and delivers them to customers.  
- **System Administrator** : Oversees the entire system, manages users, resolves disputes, and ensures smooth operations.  
- **Customer Service** : Assists customers, delivery personnel, and restaurant owners in case of issues or inquiries.  
- **Payment Gateway Provider** : Handles secure online transactions for food orders.  

### `Main use cases` 
- **Register & Authenticate Users**: 
    - Users can sign up, log in, and manage their authentication securely.
      - Customers and drivers can sign up and log in using their phone numbers.
      - Restaurant owners and their staff can sign up and log in using email and password.
   - User accounts can be activated or deactivated by either the system or the user.
     
 - **Manage Customer Profile**: 
    - A Customer can update their profile
    - A Customer can manage their addresses by add , edit & delete address & select the default
    - A Customer can add or delete saved payment methods . 
    - A Customer can manage their resturants or food preferences by adding or remove it from favorite list.
    - A Customer can Deactive their account
      
 - **Manage Restaurants**: 
    - Admins and restaurant owners can add new restaurants/branches , update restaurant/branch, Enable/Disable Restaurant/branch to the platform
    - Restaurant owners can manage the work schedules of their branches.
    - Customers can browse all available restaurants or search by name using input and filters like location, rating, and type, etc.
    - The system recommends restaurants to customers based on preferences and past activity.
    - Customers can add or remove restaurants from their favorites list.
      
 - **Manage Menus**: 
    - Restaurant owners can create, update, delete and manage menu items, including pricing and availability.
    - Restaurant owners can view the history of changes made to the restaurant’s menu.
    - Customers can search for specific menu items using filters like price, category, etc.
      
 - **Manage Cart**: 
    - Customers can add, remove, view & update quantity of items in their cart before placing an order. 
    - Customers proceed to checkout to enter shipping details, select payment methods, and confirm the order.
      
      **(For detailed specifications, including use case flows, diagrams, pseudocode , data models and others, refer to the [Manage Cart Use Case Document](./manage-cart-case.md))**
      
 - **Manage Orders**: 
    - Customers can place orders, while restaurants and delivery personnel handle order fulfillment.
    - Customers or restaurants can cancel an order before it's processed or delivered.
    - The system tracks and updates the order status ("Preparing," "On the way," "Delivered") in real-time & Notify the customer ) when there’s a change in their order status. 
    - Customers and restaurants can view their past orders, including details and statuses.
    - Customers and restaurants can view a summary of the order, including items, quantities, prices, and total amount.
    - Customers and restaurants can view detailed information for each order, such as delivery address, payment method, and special instructions.
      
      **(For detailed specifications, including use case flows, diagrams, pseudocode , data models and others , refer to the [Manage Order Use Case Document](./place-order-use-case.md))**
      
 - **Integrate Payment**: 
    - Customers can securely make payments using different methods, and the system processes transactions.
      
 - **Manage Offers & Discounts**: 
    - Admins and restaurant owners can create, apply, and update promotional offers and discounts.
      
 - **Manage Wallet**: 
    - Customers Add funds via credit card, refunds, or referral bonuses.
    - Customers can view detailed wallet transactions, including income and usage.
    - Customers can Track all wallet recharge transactions.
      
 - **Customer Service & Support**:  
    - Customers can raise issues, request refunds, or contact support for assistance.
      
 - **Manage Notifications & Alerts**: 
    - The system sends real-time notifications about order status, promotions, and updates via email, SMS, or push notifications
      
 - **Referral Code System**: 
    - Customers can share referral codes to invite new users and earn rewards.
      
 - **Loyalty Points & Rewards System**: 
    - Customers earn points based on their purchases, which can be redeemed for discounts or free items.
      
 - **Manage Dashboards**: 
    - Restaurant Dashboard – Restaurant owners can track orders, manage menus, and view performance analytics.
    - System Dashboard – Admins can monitor platform performance, user activities, and system analytics.


### `Use Case Diagram` 

A visual representation of use cases and actors

![FDS Use Case Diagram](./diagrams/food-delivery-app-use-case-modal.png) 

