def evaluate_grade(score):
    if score < 0 or score > 100:
        return "Invalid score"
    if score >= 90:
        return "A"
    elif score >= 85:
        return "A-"
    elif score >= 80:
        return "B+"
    elif score >= 75:
        return "B"
    elif score >= 70:
        return "B-"
    elif score >= 65:
        return "C+"
    elif score >= 60:
        return "C"
    elif score >= 50:
        return "D"
    else:
        return "F"
def print_grade_summary(student_name='Unnamed', score=0.0):
    grade = evaluate_grade(score)
    if grade == "Invalid score":
        print(f"Score must be between 0 and 100. You entered: {score}")
    else:
        print(f"Student {student_name} scored {score} → Grade: {grade}")
print_grade_summary(student_name='Mohib', score=91)

