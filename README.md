# Android Shipments 

Android application that assigns each shipment destination to a given driver in a way that maximizes the total suitability score for all shipments and drivers. The application displays a list of drivers and, when a driver is selected from the list, displays the shipment destination for that driver in the same cardview.


# How it works

Using the given rules, the application takes the list of drivers and the list of addresses as well and transform them into new lists of UI-readable lists.
Whenever a driver is clicked, the algorithm iterates every (available) address of the list and check its SS, then the address with the highest SS gets locked to make it unavailable for the rest of drivers as the time this address is assigned to the selected driver (that also gets locked).


## Data source

The source of information of this application comes from a .json file that is located in the /assets folder, it gets parsed using GSON.

## App architecture

This application is build using Clean Architecture and MVVM design pattern.

![MVVM with Clean Architecture: Android Apps that Scale | Toptal](https://uploads.toptal.io/blog/image/127608/toptal-blog-image-1543413671794-80993a19fea97477524763c908b50a7a.png)


