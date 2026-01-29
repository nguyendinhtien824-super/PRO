```mermaid
classDiagram
    direction LR
    
    class Pet {
        -String id
        -String name
        -int age
        -double price
        -String type
        +Pet()
        +input() void
        +display() void
    }

    class Dog {
        -String breed
        -int collarSize
        +Dog()
        +input() void
        +display() void
    }

    class Cat {
        -String breed
        -boolean climber
        +Cat()
        +input() void
        +display() void
    }

    class Customer {
        -String id
        -String name
        -String phone
        +Customer()
        +input() void
        +display() void
    }

    class Order {
        -String orderId
        -Customer customer
        -List~Pet~ petList
        +Order()
        +addPet(Pet pet) void
        +display() void
    }

    class PetStoreManagement {
        -List~Pet~ pets
        -List~Order~ orders
        +addPet() void
        +removePet() void
        +searchByName() void
    }

    class Main {
        +main(String[] args) static
    }
      
