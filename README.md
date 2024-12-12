import csv
1.

def save_to_csv(items, scores, filename="results.csv"):
    with open(filename, mode="w", newline="") as file:
        writer = csv.writer(file)
        writer.writerow(["Nosaukums", "Rezultāts"])

  for i in range(len(items)):
        writer.writerow([items[i], scores[i]])
        
#šādais kods saglāba datus CVC failā.

 



2.
 
def group_items(names, scores, threshold):
    above_threshold = []
    below_threshold = []
 for i in range(len(scores)):
        if scores[i] > threshold:
            above_threshold.append(names[i])
        else:
            below_threshold.append(names[i])

  return above_threshold, below_threshold

  №Šis kods grupē vienumus pamatojoties uz to kā tie sasniedz sliekšņa vērtību.


3.
   
def save_to_csv(items, scores, filename="results.csv"):
    with open(filename, mode="w", newline="") as file:
        writer = csv.writer(file)
        writer.writerow(["Nosaukums", "Rezultāts"])

  for i in range(len(items)):
        writer.writerow([items[i], scores[i]])


4.
def calculate_statistics(grades):
    if not grades:
        return 0, 0, 0

total = sum(grades)
count = len(grades)
average = total / count
highest = max(grades)
lowest = min(grades)

return average, highest, lowest

grades_list = [5, 7, 8, 10, 6]
average, highest, lowest = calculate_statistics(grades_list)
print("Vidējā:", average)
print("Augstākā:", highest)
print("Zemākā:", lowest)

#Šādais kods ir labs lai rēķināt skolniekas atzīmes.

5.

def print_statistics(average, highest, lowest):
    print(f"Vidējais rezultāts: {average:.2f}")
    print(f"Augstākais rezultāts: {highest}")
    print(f"Zemākais rezultāts: {lowest}")
    
#šitais kods ievada statistiku

6.

def print_animal_groups(above_average, below_average):
    print("Dzīvnieki virs vidējā līmeņa:", above_average)
    print("Dzīvnieki zem vidējā līmeņa:", below_average)

#kods rāda 2 dzivniekus grupas



7.

if __name__ == "__main__":
    animals = ["Lācis", "Vilks", "Zaķis", "Vārna", "Lūsis"]
    levels = [8, 6, 9, 5, 7]

   average, highest, lowest = calculate_statistics(levels)

   print_statistics(average, highest, lowest)

  above_average, below_average = group_animals(animals, levels, average)

  print_animal_groups(above_average, below_average)

  save_to_csv(animals, levels)
    print("Rezultāti saglabāti 'results.csv' failā.")

  #šis kods manipulē ar dzīvnieku datiem, parsē to līmeņus, grupē tos pēc līmeņa un saglabā rezultātus failā.

        
























