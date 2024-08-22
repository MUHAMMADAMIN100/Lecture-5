# Массив В JavaScript
## Что такое массив?
### Массивы в JavaScript – это некая структура данных, ориентированная на хранение различных элементов, зачастую однотипных. Их главная особенность состоит в том, что они позволяют хранить некоторое количество значений в одной переменной.
![Image](./Массив.jpg)

## Элементы массива нумеруются, начиная с нуля.
### Мы можем получить элемент, указав его номер в квадратных скобках:
![Image](./massiv%20index.png)
### Мы можем заменить элемент:
![Image](./massiv%20zamena.png)
### Или добавить новый к существующему массиву:
![Image](./massiv%20dobav.png)
# Методы Массива
# Метод pop
## Метод pop удаляет последний элемент из массива. При этом исходный массив изменяется, а результатом метода возвращается удаленный элемент.
## Пример 1
### Давайте удалим из массива последний элемент:
![Image](./massiv%20pop.png)
## Пример 2
### Давайте выведем последний элемент, который был удален из исходного массива:
![Image](./massiv%20pop%20ex2.png)  

# Метод push
## Метод push добавляет неограниченное количество элементов в конец массива. При этом исходный массив изменяется, а результатом возвращается новая длина массива.
## Пример 1
### Давайте в конец массива добавим еще два новых элемента:
![Image](./massiv%20push.png)  
## Пример 2
### Добавим в массив два новых элемента и выведем новую длину массива:
![Image](./massiv%20push%20ex%202.png) 
# Метод unshift
## Метод unshift добавляет неограниченное количество новых элементов в начало массива. При этом исходный массив изменяется, а результатом возвращается новая длина массива.
## Пример 1
### Давайте в начало массива добавим еще два новых элемента и выведем измененный массив:
![Image](./massiv%20unshift.png) 
## Пример 2
### Давайте добавим два новых элемента и выведем новую длину массива:
![Image](./massiv%20unshift%20ex%202.png) 
# Метод shift
## Метод shift удаляет первый элемент из массива. При этом исходный массив изменяется, а результатом метода возвращается удаленный элемент.
## Пример 1
### Давайте удалим первый элемент из массива:
![Image](./massiv%20shift.png) 
## Пример 2
### Давайте удалим первый элемент из массива и выведем его на экран:
![Image](./massiv%20shift%20ex%202.png) 
# Метод toString
## Метод toString() также может быть использован для преобразования массивов в строки. В этом случае элементы массива будут объединены в одну строку, разделенную запятыми.
![Image](./massiv%20tostring.png) 
# Метод indexOf
## Метод indexOf осуществляет поиск элемента в массиве. В первом параметре указываем номер позиции искомого символа. Метод возвращает номер первого найденного элемента, либо -1, если такого элемента нет. Второй необязательный параметр метода задает позицию, с которой следует начинать поиск.
## Пример 1
### Давайте найдем позицию первой тройки в массиве:
![Image](./massiv%20indexof.png)
 ## Пример 2
 ### Пусть теперь проверяемого элемента нет в массиве:
 ![Image](./massiv%20indexof%20ex%202.png)
 # Метод includes
 ## Метод includes проверяет наличие элемента в массиве. Параметром принимает значение для поиска. Если такой элемент есть в массиве, то метод возвращает true, а если нет, то false.
 ## Пример 1
 ### Давайте проверим наличие элемента в массиве:
 ![Image](./massiv%20includes.png)
 ## Пример 2
 ### Пусть теперь проверяемого элемента нет в массиве:
  ![Image](./massiv%20includes%20ex%202.png)
  # Метод concat
  ## Метод concat сливает указанные массивы в один общий массив. Метод применяется к одному из массивов, а в параметрах метода передаются остальные массивы для слияния. При этом метод не изменяет исходный массив, а возвращает новый.
  ## Пример 1
  ### Давайте сольем 3 массива в один с помощью метода concat:
   ![Image](./massiv%20concat.png)
## Пример 2
### А теперь давайте сольем два массива вместе:
 ![Image](./massiv%20concat%20ex%202.png)
# Метод slice
## Метод slice вырезает и возвращает указанную часть массива. Сам массив при этом не изменяется.

## Первым параметром указывается номер элемента массива, с которого начинается вырезание, а вторым параметром - номер элемента, на котором закончится вырезание (при этом элемент с этим номером не включится в вырезанную часть). Второй параметр не является обязательным. Если его не указать - подмассив возьмется с указанного в первом параметре элемента до конца массива.

## Он также может принимать отрицательные значения. В этом случае отсчет элемента, на котором закончится обрезание, начинается с конца массива. Последний элемент при этом будет иметь номер -1.
## Пример 1
### Давайте вырежем из массива элементы с нулевого по второй не включительно (второй не вырежется)
![Image](./massiv%20slice%20ex%201.png)
## Пример 2
### Давайте вырежем с первого элемента до конца массива. Для этого второй параметр не задаем:
![Image](./massiv%20slice%20ex%202.png)
## Пример 3
### Давайте вырежем элементы со второго по предпоследний (-1 указывает на последний элемент и он не включится в извлеченную часть):
![Image](./massiv%20slice%20ex%203.png)
+ Преимущество такого подхода в том, что вырезаться всегда будет часть массива, не включая последний элемент, независимо от размера массива.
# Метод splice
## Метод splice удаляет или добавляет элементы в массив. Можно только удалять элементы, только добавлять или делать и то и другое одновременно. Метод очень универсальный и сложный для понимания. Метод изменяет сам массив и возвращает при этом массив удаленных элементов.

## Первым параметром метод принимает номер элемента массива, который нужно удалить. Вторым параметром - сколько элементов массива следует удалить. Если его поставить в 0 - то элементы удалены не будут (только добавлены новые). Дальше через запятую идут элементы, которые нужно добавить в массив (являются необязательными параметрами). Эти элементы добавятся вместо удаленных элементов массива.

## Если удаления не было (когда второй параметр 0) - элементы вставятся в массив начиная с той позиции, которая указана первым параметром метода. Первый параметр может иметь отрицательное значение. В этом случае отсчет позиции начнется не с начала массива, а с конца. Последний элемент при этом будет иметь номер -1.
## Пример 1
### Давайте удалим три элемента, начиная с первого:
![Image](./massiv%20splice%20ex1.png)
## Пример 2
### Давайте выведем массив удаленных элементов:
![Image](./massiv%20splice%20ex%202.png)
## Пример 3
### Давайте сначала удалим элемент с номером 2, а потом вместо него вставим еще три новых элемента:
![Image](./massiv%20splice%20ex%203.png)
## Пример 4
### Давайте теперь ничего не будем удалять, но на позицию 2, вставим еще три новых элемента:
![Image](./massive%20splice%20ex%204.png)
## Пример 5
### Давайте удалим предпоследний элемент:
![Image](./massive%20splice%20ex%205.png)
# Метод map
## Метод map позволяет применить заданную функцию для каждого элемента массива. При этом метод не изменяет исходный массив, а возвращает измененный.

 ## Метод в параметре получает функцию, которая выполнится для каждого элемента массива. То, что вернет эта функция через return для элемента массива, станет новым значением этого элемента (см. примеры).

## В функцию можно передавать 3 параметра. Если эти параметры есть (они не обязательны), то в первый автоматически попадет элемент массива, во второй попадет его номер в массиве (индекс), а в третий - сам массив.
## Пример 5
### Создадим массив, каждый элемент которого вдвое больше соответствующего элемента начального массива:
![Image](./massive%20splice%20ex%205.png)
# Метод forEach
## Метод forEach позволяет последовательно перебрать все элементы массива. Метод в параметре получает функцию, которая выполнится для каждого элемента массива.

## В эту функцию можно передавать три параметра. Если эти параметры есть (они не обязательны), то в первый автоматически попадет элемент массива, во второй попадет его номер в массиве (индекс), а в третий - сам массив.
## Пример 
### Давайте найдем сумму элементов массива:
![Image](./massiv%20foreach.png)
# Метод find
## Метод find помогает найти первый элемент в массиве согласно переданному в параметре коллбэку. Если элемента нет, то возвращается undefined.
## Пример 1
### Давайте найдем элемент массива, соответствующий условиям, прописанным в функции:
![Image](./massive%20find.png)
## Пример 2
### Давайте найдем элемент массива, длина которого равна 2:
![Image](./massiv%20find%20ex%202.png)
# Метод filter
## Метод filter позволяется отфильтровать элементы массива, оставив только подходящие под определенное условие элементы. Метод в параметре получает функцию, которая выполнится для каждого элемента массива. Своим результатом метод возвращает новый массив, в который войдут только те элементы, для которых переданная функции вернет true.

 ## В функцию можно передавать три параметра. Если эти параметры есть (они не обязательны), то в первый автоматически попадет элемент массива, во второй попадет его номер в массиве (индекс), а в третий - сам массив.

## Пример 1
### Давайте отфильтруем массив, оставив в нем только положительные числа:
![Image](./massive%20filter.png)


# Метод toSorted
## Метод массива toSorted() это копия метода sort(), но, в отличие от него, не мутирует исходный массив, а возвращает новый отсортированный массив. Все undefined элементы сортируются в конец массива.
# Пример
![Image](./massive%20toSorted.png)
# Метод reduce
## Метод reduce сворачивает массив к одному значению (редуцирует). К примеру, с помощью этого метода можно легко найти сумму элементов массива (то есть массив сведется к одному значению - к сумме элементов).

## Первым параметром метод reduce получает функцию, которая последовательно выполнится для каждого элемента массива, начиная с первого. В эту функцию можно передавать 4 параметра. Если эти параметры есть (они не обязательны), то в первый автоматически попадет промежуточный результат, во второй попадет элемент массива, в третий - его номер в массиве (индекс), а в четвертый - сам массив.

## Промежуточный результат - это переменная, в которой будет накапливаться то значение, которое вернет метод reduce, когда переберет все элементы массива. К примеру, туда последовательно можно накапливать сумму элементов массива: сначала положить первый элемент, при следующем проходе цикла уже сумму первого элемента и второго, при следующем проходе - сумму первого, второго и третьего. И так, пока массив не закончится. Функция, которую принимает reduce, должна возвращать новое значение промежуточного результата.

## Вторым параметром метода reduce указывается начальное значение промежуточного результата. Если его не указать, то оно будет равно первому элементу массива, а обработка элементов начнется со второго элемента.
# Пример 1
## Найдем сумму элементов массива:

![Image](./massive%20reduce.png)
# Пример 2
## Давайте найдем сумму всех положительных чисел массива:
![Image](./massive%20reduce%20ex%202.png)
# Метод Destruction
## Деструктуризация (destructuring assignment) – это особый синтаксис присваивания, при котором можно присвоить массив или объект сразу нескольким переменным, разбив его на части.
# Пример 1
![Image](./massiv%20destruction%20ex%201.png)

+ При таком присвоении первое значение массива пойдёт в переменную firstName, второе – в lastName, а последующие (если есть) – будут отброшены.
# Пример 2
## Ненужные элементы массива также можно отбросить, поставив лишнюю запятую:
![Image](./massiv%20destruction.png)
# Метод spread
## Спред-синтаксис (spread) ... позволяет передавать итерируемые коллекции (например, массивы или строки) как список аргументов функции или добавлять содержащиеся в них элементы в новый массив.
# Пример 
![Image](./massive%20spred.png)
# Метод rest
## rest- позволяет представлять неограниченное множество аргументов в виде массива.
![Image](./massive%20rest.png)