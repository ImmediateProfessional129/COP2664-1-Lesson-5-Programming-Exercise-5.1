# COP2664-1-Lesson-5-Programming-Exercise-5.1
This repository link is a submission link for COP264-1: Lesson 5 Programming Exercise 5.1

// This program is designed for a user to add an item to their shopping list and the program will print out the list for both the cart and the wishlist. Plus, they can also remove any item they want off the shopping cart list and place it in the wishlist instead.

import Foundation // Imports the Foundation library
var shoppingCart: Set<String> = [] // Creates an empty set for the shopping cart
var wishlist: Set<String> = [] // Creates an empty set for the wishlist
func addItem(item: String) { // Creates a function to add an item to the shopping cart
    shoppingCart.insert(item) // Adds the item to the shopping cart
}
func removeItem(item: String) { // Creates a function to remove an item from the shopping cart
    shoppingCart.remove(item) // Removes the item from the shopping cart
}
func printItems() { // Creates a function to print the items in the shopping cart and wishlist
    print("Shopping Cart:") // Prints the title for the shopping cart
    for item in shoppingCart { // Iterates through the shopping cart
        print(item) // Prints each item in the shopping cart
    }
}
func addItemToWishlist(item: String) { // Creates a function to add an item to the wishlist
    wishlist.insert(item) // Adds the item to the wishlist
}
func printWishlist() { // Creates a function to print the items in the wishlist
    print("Wishlist:") // Prints the title for the wishlist
    for item in wishlist { // Iterates through the wishlist
        print(item) // Prints each item in the wishlist
    }
}
func findIntersection() { // Creates a function to find the intersection of the shopping cart and wishlist
    let intersection = shoppingCart.intersection(wishlist) // Finds the intersection of the shopping cart and wishlist
    print("Items in both cart and wishlist: 9") // Prints the title for the intersection
    for item in intersection { // Iterates through the intersection
        print(item) // Prints each item in the intersection
    }
}
func findDifference() { // Creates a function to find the difference between the shopping cart and wishlist
    let difference = shoppingCart.subtracting(wishlist) // Finds the difference between the shopping cart and wishlist
    print("Items only in the wishlist, not yet in the cart: 4") // Prints the title for the difference
    for item in difference { // Iterates through the difference
        print(item) // Prints each item in the difference
    }
}
addItem(item: "Grapefruits") // Adds "Grapefruits" to the shopping cart
addItem(item: "Strawberries") // Adds "Strawberries" to the shopping cart
addItem(item: "Blueberries") // Adds "Blueberries" to the shopping cart
addItem(item: "Cherries") // Adds "Cherries" to the shopping cart
addItem(item: "Lemons") // Adds "Lemons" to the shopping cart
printItems() // Prints the items in the shopping cart
removeItem(item: "Grapefruits") // Removes "Grapefruits" from the shopping cart
printItems() // Prints the items in the shopping cart
addItemToWishlist(item: "Grapefruits") // Adds "Grapefruits" to the wishlist
addItemToWishlist(item: "Apples") // Adds "Apples" to the wishlist
addItemToWishlist(item: "Bananas") // Adds "Bananas" to the wishlist
addItemToWishlist(item: "Raspberries") // Adds "Raspberries" to the wishlist
printWishlist() // Prints the items in the wishlist
findIntersection() // Finds the intersection of the shopping cart and wishlist
findDifference() // Finds the difference between the shopping cart and wishlist
