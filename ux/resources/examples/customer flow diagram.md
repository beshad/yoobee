```mermaid
graph TD
        Start((START)) --> Home_Page[Home Page]
        Home_Page --> Explore[Explore Products]
        Explore --> Select[Select Category]
       View_Product ---> View_Reviews[View Reviews]
        Select --> View_Product[View Product]
        View_Product --> Add_to_Cart{Add to Cart}
        Add_to_Cart -->|Yes| View_Cart[View Cart]
        Add_to_Cart -->|No| Explore
        View_Cart --> Checkout[Checkout]
        Checkout --> Are_You{Are You Registered?}
        Are_You -->   |Yes|Login --> Shipping
        Shipping --> Payment[Payment Method]
        Payment --> Review[Review Order]
        Review --> Place[Place Order]
        Place --> End
        Home_Page --> View_Blog[View Blog Posts]
        Home_Page --> Contact[Contact Us]
        Contact --> End((End))
        Are_You -->|No| Register[Register Account]
        Register --> Shipping
        Place --> Home_Page