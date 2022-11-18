# import table libery
from tabulate import tabulate
# the function that convert grade from degree to letters
def letter_grade(degree):
  if   degree >= 95: return "A+"
  elif degree >= 90: return "A"
  elif degree >= 85: return "B+"
  elif degree >= 80: return "B"
  elif degree >= 75: return "C+"
  elif degree >= 70: return "C"
  elif degree >= 65: return "D+"
  elif degree >= 60: return "D"
  else: return "F"
# display top of table
stu_config = [["Student Name", "Percentage Grade", "Letter Grade"]]
# take number of student
stu_num = int(input("Enter How many student: "))
if stu_num <= 0: # checking that number is not zero or negative
  print("number of student not correct!")
else:
  for c in range(stu_num):
    # take name of student
    stu_name = str(input("Enter Student Name: "))
    # take grade of student
    stu_grade = int(input("Enter Student Grade: "))
    # insert the information of students
    stu_config.append([stu_name, stu_grade, letter_grade(stu_grade)]) 
  # display the name, grade(Percentage), grade(Letter) of the students
  print("\nStudent Grade:")
  print(tabulate(stu_config, headers='firstrow', tablefmt='fancy_grid', showindex=range(1, stu_num+1)))
