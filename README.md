# Movie-List
This is a movie watch list, where you can add a movie, mark it as watched, and more. 

#initialize

#functions

#main
def movieList():
    movielist = []
    while True:
        choice = input("What would you like to do? 1 - add, 2- view, 3 - mark as complete, 4- remove, 5- exit ")
        if choice == "1":
            ListItem = input("What do you want to add to the list? ")
            movielist.insert(0,ListItem)
        elif choice == "2":
            print(movielist)
        elif choice == "3":
            CompleteListItem = int(input("What item on the list is complete? "))
            movielist.insert(CompleteListItem,"X")
        elif choice == "4":
            RemoveListItem = input("What item would you like to remove? ")
            movielist.remove(RemoveListItem)
        elif choice == "5":
            break

movieList()
