## Описание интерфейса IDriver
Интерфейс предназначен для работы с методами класса [Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md)
## Реализация интерфейса
* Add (Driver: [Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md)) — функция, добавляющая водителя в базу данных. Параметр «Driver» — водитель, которого необходимо добавить в БД;
* Del (Driver: [Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md)) — функция, удаляющая водителя из программы. Параметр «Driver» — водитель, которого необходимо удалить из программы;
* Edit (Driver: [Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md)) — функция, редактирующая данные о водителе. Параметр «Driver» — водитель, которого необходимо редактировать в БД;
* FindByID< [Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md) >(ID : Integer) : Driver — функция, осуществляющая поиск водителя в базе данных по ID и возвращающая найденного водителя, если такой имеется. 
* GetID(Driver: [Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md)) : Integer — функция, возвращающая ID определенного водителя. 
* GetDriverDel(Date1:DateTime,Date2:DateTime):List<[Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md)> - функция, возвращающая список доставок водителя в определенном временном промежутке.
* GetSchedule(Date1:DateTime,Date2:DateTime): List<String> - функция, возвращающая маршрут водителя.
* Get Driver (sorting : String, ASKorDESK : string, filterA : Driver,  ilter : Driver, count : int, page : int) : List < [Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md) > — функция, возвращающая список водителей с заданными параметрами.
 Параметры: 
-	sortintg: String– отвечает, по какому полю будет сортироваться список:
-	ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
-	filterA : [Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md) – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
-	 filterB : [Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md) – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
-	count : Integer – отвечает, сколько элементов необходимо показать;
-	page: Integer – отвечает, с какой страницы начинать поиск элементов.
