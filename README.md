```
# Эталонное множество
X = {1, 2, 3, 4, 5}

# Другие множества
A = {1, 2, 6, 7}
B = {3, 4, 5, 8}
C = {9, 10, 11}

# Создадим словарь для хранения размеров пересечений
intersections = {
    "A": len(A.intersection(X)),
    "B": len(B.intersection(X)),
    "C": len(C.intersection(X))
}

# Найдём множество с максимальным количеством совпадений
best_set = max(intersections, key=intersections.get)
max_count = intersections[best_set]

print(f"Множество с наибольшим количеством совпадений: {best_set}")
print(f"Количество совпадений: {max_count}")
```
