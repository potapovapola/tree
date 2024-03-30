# tree
class Tree:
    def __init__(self, species, height, age):
        self.species = species
        self.height = height
        self.age = age

    def grow(self, growth_rate):
        self.height += growth_rate

    def display_info(self):
        return f"Species: {self.species}, Height: {self.height} meters, Age: {self.age} years"

def main():
    # Creating a tree instance
    my_tree = Tree("Oak", 5, 10)

    # Displaying tree information
    print("Before growth:")
    print(my_tree.display_info())

    # Simulating growth
    my_tree.grow(0.5)

    # Displaying updated tree information
    print("\nAfter growth:")
    print(my_tree.display_info())

if __name__ == "__main__":
    main()
