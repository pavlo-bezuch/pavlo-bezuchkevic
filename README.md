hello = "Hello World"
name = "Pavlo"
last_name = "Bezushkevych"
age = 16

print(hello)
print(name)
print(last_name)
print(age)

types_list = [type(hello), type(name), type(last_name), type(age)]

print("Types of variables:", types_list)


if all(t == types_list[0] for t in types_list):
    print("Good")
else:
    common_type = types_list[0]
    filtered_types = [t for t in types_list if t == common_type]
    print("Filtered types:", filtered_types)
