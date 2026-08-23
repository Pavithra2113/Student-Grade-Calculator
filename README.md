# Student Grade Calculator

name = input("Enter Student Name: ")

marks = []
subjects = ["Maths", "Science", "English", "Computer", "Social"]

for subject in subjects:
    mark = float(input(f"Enter {subject} mark: "))
    marks.append(mark)

total = sum(marks)
average = total / len(marks)

if average >= 90:
    grade = "A+"
elif average >= 80:
    grade = "A"
elif average >= 70:
    grade = "B"
elif average >= 60:
    grade = "C"
else:
    grade = "D"

print("\n----- RESULT -----")
print("Name:", name)
print("Total:", total)
print("Average:", round(average,2))
print("Grade:", grade)
