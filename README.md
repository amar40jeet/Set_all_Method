# Starting with an empty set
my_set = set()

# 1. add(): Add an element to the set
my_set.add(1)
my_set.add(2)
my_set.add(3)
print("After add:", my_set)  # Output: {1, 2, 3}

# 2. update(): Update the set with elements from another iterable
my_set.update([4, 5])
print("After update:", my_set)  # Output: {1, 2, 3, 4, 5}

# 3. remove(): Remove an element from the set. Raises KeyError if the element is not present
my_set.remove(3)
print("After remove:", my_set)  # Output: {1, 2, 4, 5}

# 4. discard(): Remove an element from the set if it is present. Does nothing if the element is not present
my_set.discard(2)
print("After discard:", my_set)  # Output: {1, 4, 5}

# 5. pop(): Remove and return an arbitrary element from the set
popped_element = my_set.pop()
print("After pop:", my_set)        # Output: Set with one element removed
print("Popped element:", popped_element)

# 6. clear(): Remove all elements from the set
my_set.clear()
print("After clear:", my_set)  # Output: set()

# Restore the set with some elements
my_set = {1, 2, 3, 4, 5}

# 7. copy(): Create a shallow copy of the set
copied_set = my_set.copy()
print("Copied set:", copied_set)  # Output: {1, 2, 3, 4, 5}

# 8. union(): Return a new set with elements from the set and another iterable
another_set = {4, 5, 6, 7}
union_set = my_set.union(another_set)
print("Union of sets:", union_set)  # Output: {1, 2, 3, 4, 5, 6, 7}

# 9. intersection(): Return a new set with elements common to the set and another iterable
intersection_set = my_set.intersection(another_set)
print("Intersection of sets:", intersection_set)  # Output: {4, 5}

# 10. difference(): Return a new set with elements in the set that are not in another iterable
difference_set = my_set.difference(another_set)
print("Difference of sets:", difference_set)  # Output: {1, 2, 3}

# 11. symmetric_difference(): Return a new set with elements in either the set or another iterable but not both
symmetric_difference_set = my_set.symmetric_difference(another_set)
print("Symmetric difference of sets:", symmetric_difference_set)  # Output: {1, 2, 3, 6, 7}

# 12. issubset(): Check if the set is a subset of another set
is_subset = my_set.issubset({1, 2, 3, 4, 5, 6, 7})
print("Is subset:", is_subset)  # Output: True

# 13. issuperset(): Check if the set is a superset of another set
is_superset = my_set.issuperset({1, 2})
print("Is superset:", is_superset)  # Output: True

# 14. isdisjoint(): Check if the set has no elements in common with another set
is_disjoint = my_set.isdisjoint({6, 7})
print("Is disjoint with {6, 7}:", is_disjoint)  # Output: False
