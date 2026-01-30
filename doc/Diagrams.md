```mermaid
classDiagram
    direction TD
    %% Định nghĩa các lớp con (Nằm trên)
    class Fish {
        -finType: String
        -isAggressive: boolean
        +Fish()
        +input() : void
        +display() : void
    }

    class AquaticPlant {
        -lightRequirement: String
        -growthRate: String
        +AquaticPlant()
        +input() : void
        +display() : void
    }

    %% Định nghĩa lớp cha (Nằm dưới)
    class AquaticProduct {
        -id: String
        -name: String
        -price: double
        -waterType: String
        +AquaticProduct()
        +AquaticProduct(id, name, price, waterType)
        +input() : void
        +display() : void
        +getPrice() : double
        +getId() : String
        +getName() : String
    }

    %% Mối quan hệ: Con trỏ xuống Cha (Dùng mũi tên --> để giống hình mẫu)
    Fish --> AquaticProduct
    AquaticPlant --> AquaticProduct
