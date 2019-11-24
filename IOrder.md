## Описание интерфейса IOrder
Интерфейс предназначен для работы с методами класса [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md)
## Реализация интерфейса
* Add (Order: [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md)) — функция, добавляющая заказ в базу данных. Параметр «Order» — заказ, который необходимо добавить в БД;
* Del (Order: [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md)) — функция, удаляющая заказ из программы. Параметр «Order» — заказ, который необходимо удалить из программы;
* Edit (Order: [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md)) — функция, редактирующая данные о заказе. Параметр «Order» — заказ, который необходимо редактировать в БД;
* FindByID< [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md) >(ID : Integer) : Order — функция, осуществляющая поиск заказа в базе данных по ID и возвращающая найденный Order, если такой имеется. 
* GetID(Order: [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md)) : Integer — функция, возвращающая ID определенного заказа. 
* GetOrder (sorting : String, ASKorDESK : string, filterA : [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md), filterB : [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md), count : int, page : int) : List < [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md) > — функция, возвращающая список заказов с заданными параметрами.
* GetBestDish(Date1:DateTime,Date2:DateTime):List<[Menu](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Menu.md)> - функция, возвращающая топ список блюд в определенном временном промежутке. 
 Параметры: 
-	sortintg: String– отвечает, по какому полю будет сортироваться список:
-	ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
-	filterA : [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md) – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
-	filterB : [Order](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Order.md) – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
-	count : int – отвечает, сколько элементов необходимо показать;
-	page: int – отвечает, с какой страницы начинать поиск элементов.

