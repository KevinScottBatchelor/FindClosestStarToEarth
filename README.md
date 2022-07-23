# FindClosestStarToEarth

The purpose of this program is to conceptualize the idea of 'defining' star objects with the Star class and then using a method that takes the giant list of stars in the known-universe and an int k that will find k amount of 'stars closest to earth.'

This uses an array data structure to hold the Star objects (I'm still learning so I know that there are better choices out there, but this is something that I can get my idea across for now).

I have two methods of approaching the problem:

Method #1: Uses nested for loops and the public static final double MAX_VALUE (A constant holding the largest positive finite value of type double, (2-2-52)·21023) to use as a placeholder for comparing the distanceFromEarth. The idea here is that the variable minDistance is set to the largest possible number that the data type double can hold and then each star in the list is compared to this value. Each star object's distanceFromEarth is compared to the 'furthest away' distance of minDistance and if the star being compared is closer to Earth, the minDistance variable is assigned to the 'closer value' and gets added to the closestStars list of size k.
