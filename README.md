# markdown-formatting
#Sep 18,2023
---
##Relation 1

|**Vehicleid**|**VehicleType**|
|---          |---            |
|001          |Bike           |
|002          |Car            |
|003          |Van            |
|004          |Jeep           |

##Relation 2

|**Vehicleid**|**SparepartName**|
|---          |---            |
|001          |Bike Motor          |
|002          |Car Pump            |
|003          |Van Tyre           |
|004          |Jeep Buffer          |

`Find the relation of VehicleType=SparepartName`

##Cross Product

##Relation 1 X Relation 2

|**Vehicleid**|**VehicleType**|**Vehicleid**|**SparepartName**|
|---          |---            |---	    |---	      |
|001          |Bike           |001          |Bike Motor       |
|002          |Car            |001          |Bike Motor       |
|003          |Van            |001          |Bike Motor       |
|004          |Jeep           |001          |Bike Motor       |
|001          |Bike           |002          |Car pump       |
|002          |Car            |002          |Car Pump       |
|003          |Van            |002          |Car pump       |
|004          |Jeep           |002          |Car pump       |
|001          |Bike           |003          |Van Tyre       |
|002          |Car            |003          |Van Tyre       |
|003          |Van            |003          |Van Tyre       |
|004          |Jeep           |003          |Van Tyre       |
|001          |Bike           |004          |Jeep Buffer      |
|002          |Car            |004          |Jeep Buffer      |
|003          |Van            |004          |Jeep Buffer      |
|004          |Jeep           |004          |Jeep Buffer      |

##Filter 

>Relation 1.**Vehicleid**=Relation 2.**Vehicleid**

|**Vehicleid**|**VehicleType**|**Vehicleid**|**SparepartName**|
|---          |---            |---	    |---	      |
|001          |Bike           |001          |Bike Motor       |
|002          |Car            |002          |Car Pump       |
|003          |Van            |003          |Van Tyre       |
|004          |Jeep           |004          |Jeep Buffer      |

##Projection

>(VehicleType,SparepartName)

|**VehicleType**|**SparepartName**|
|---            |---            |
|Bike           |Bike Motor      |
|Car            |Car Pump         |
|Van            |Van Tyre         |
|Jeep            |Jeep Buffer      |























