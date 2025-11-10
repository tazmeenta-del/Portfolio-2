# Portfolio-2
def calculate_grade(marks):
    total_marks = sum(marks)
    percentage = (total_marks / 300) * 100

    if percentage >= 80:
        grade = "A"
    elif percentage >= 70:
        grade = "B"
    elif percentage >= 60:
        grade = "C"
    elif percentage >= 40:
        grade = "D"
    else:
        grade = "Fail"

    return total_marks, percentage, grade

def main():
    print("Enter marks for three subjects:")
    subject1 = float(input("Subject 1: "))
    subject2 = float(input("Subject 2: "))
    subject3 = float(input("Subject 3: "))

    marks = [subject1, subject2, subject3]
    total_marks, percentage, grade = calculate_grade(marks)

    print("\nResults:")
    print(f"Total Marks: {total_marks} / 300")
    print(f"Percentage: {percentage:.2f}%")
    print(f"Grade: {grade}")

if __name__ == "__main__":
    main()
