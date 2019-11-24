## Описание интерфейса IEmployee
Интерфейс предназначен для работы с методами класса [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md)
## Реализация интерфейса
* Add (Employee: [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md)) — функция, добавляющая работника в базу данных. Параметр «Employee» — работник, которого необходимо добавить в БД;
* Del (Employee: [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md)) — функция, удаляющая работника из программы. Параметр «Employee» — работник, которого необходимо удалить из программы;
* Edit (Employee: [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md)) — функция, редактирующая данные о работнике. Параметр «Employee» — работник, которого необходимо редактировать в БД;
* FindByID< [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md) >(ID : Integer) : Employee — функция, осуществляющая поиск работника в базе данных по ID и возвращающая найденного работника, если такой имеется. 
* GetID(Employee: [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md)) : Integer — функция, возвращающая ID определенного работника. 
* GetEmployee(sorting : String, ASKorDESK : string, filterA : [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md), filterB : [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md), count : int, page : int) : List < Employee > — функция, возвращающая список работников с заданными параметрами.
 Параметры: 
-	sortintg: String – отвечает, по какому полю будет сортироваться список:
-	ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
-	filterA : [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md) – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
-	filterB : [Employee](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Employee.md) – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
-	count : Integer – отвечает, сколько элементов необходимо показать;
-	page: Integer – отвечает, с какой страницы начинать поиск элементов.
