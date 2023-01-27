# ex_1_vet_classes_and_objects
Create a class called Vet. Upon initialization, it should receive a name (string). It should also have an instance attribute called animals (empty list by default). There should also be 2 class attributes: animals (empty list) which will store the total amount of animals for all vets; and space (5 by default). You should create 3 additional instance methods:

- register_animal(animal_name)

o If there is space in the vet clinic, adds the animal to both animals' lists and returns a message: "{name} registered in the clinic"

o Otherwise, returns "Not enough space"

- unregister_animal(animal_name)

o If the animal is in the clinic, removes it from both animals' lists and returns "{animal} unregistered successfully"

o Otherwise, returns "{animal} not in the clinic"

- info()

o Returns info about the vet, the number of animals in his list and the free space in the clinic:

"{vet_name} has {number_animals} animals. {space_left_in_clinic} space left in clinic"



Test Code
peter = Vet("Peter")

george = Vet("George")

print(peter.register_animal("Tom"))

print(george.register_animal("Cory"))

print(peter.register_animal("Fishy"))

print(peter.register_animal("Bobby"))

print(george.register_animal("Kay"))

print(george.unregister_animal("Cory"))

print(peter.register_animal("Silky"))

print(peter.unregister_animal("Molly"))

print(peter.unregister_animal("Tom"))

print(peter.info())

print(george.info())




Output


Tom registered in the clinic Cory registered in the clinic Fishy registered in the clinic Bobby registered in the clinic Kay registered in the clinic Cory unregistered successfully Silky registered in the clinic Molly not in the clinic Tom unregistered successfully Peter has 3 animals. 1 space left in clinic George has 1 animals. 1 space left in clinic
