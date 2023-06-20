# ddd
sss
class Student:
    """学生类"""

    def __init__(self, name, age):
        self.name = name
        self.age = age
        self.grades = []

    def add_grade(self, grade):
        """添加成绩"""
        self.grades.append(grade)

    def get_average_grade(self):
        """计算平均成绩"""
        if len(self.grades) == 0:
            return 0
        return sum(self.grades) / len(self.grades)


# 创建学生对象
student1 = Student("Alice", 18)
student2 = Student("Bob", 19)

# 添加成绩
student1.add_grade(85)
student1.add_grade(90)
student2.add_grade(92)
student2.add_grade(88)

# 打印学生信息和平均成绩
print(f"{student1.name}: 平均成绩 {student1.get_average_grade()}")
print(f"{student2.name}: 平均成绩 {student2.get_average_grade()}")
