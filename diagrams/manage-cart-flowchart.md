flowchart TD
    A[Customer Opens App] --> B[Select Address\n(Auto/Manual)]
    B --> C{Authenticated?}
    C -->|No| D[Redirect to Login/Register\n(OTP Flow)]
    C -->|Yes| E[Display Restaurants\nBased on Address]
    D --> E
    E --> F[Select Restaurant &\nBrowse Menu]
    F --> G[Customize Item\n(Size, Toppings, Notes)]
    G --> H[Add Item to Cart\n(Cart Badge Updates)]
    H --> I[Open Cart]
    I --> J[Cart Management]
    
    subgraph J[Cart Management]
        J1[Update Quantity]
        J2[Remove Item]
        J3[Add Special Notes]
        J4[Clear Entire Cart]
        J5[Save Cart for Later]
        J6[Proceed to Checkout]
    end

    J1 --> K[System Updates Cart\n(Dynamic Total)]
    J2 --> K
    J3 --> K
    J4 --> K
    J5 --> K
    J6 --> L[Place Order Flow]

    K --> M{Ready to Checkout?}
    M -->|No| F
    M -->|Yes| L
