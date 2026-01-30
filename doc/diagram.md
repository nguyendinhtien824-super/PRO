```mermaid
classDiagram

class AquaticProduct {
  -id : String
  -name : String
  -price : double
  -waterType : String

  +AquaticProduct()
  +AquaticProduct(id, name, price, waterType)
  +input() : void
  +display() : void
  +getPrice() : double
  +getId() : String
  +getName() : String
}

class Fish {
  -id : String
  -name : String
  -price : double
  -waterType : String
  -finType : String
  -isAggressive : boolean

  +Fish()
  +input() : void
  +display() : void
}

class AquaticPlant {
  -id : String
  -name : String
  -price : double
  -waterType : String
  -lightRequirement : String
  -growthRate : String

  +AquaticPlant()
  +input() : void
  +display() : void
}

 
