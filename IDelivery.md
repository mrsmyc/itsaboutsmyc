## Описание интерфейса IDelivery
Интерфейс предназначен для работы с методами класса [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md)
## Реализация интерфейса
* Add (Delivery: [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md)) — функция, добавляющая доставку в базу данных. Параметр «Delivery» — доставка, которую необходимо добавить в БД;
* Del (Delivery: [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md)) — функция, удаляющая доставку из программы. Параметр «Delivery» — доставка, которую необходимо удалить из программы;
* Edit (Delivery: [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md)) — функция, редактирующая данные о доставке. Параметр «Delivery» — доставка, которую необходимо редактировать в БД;
* FindByID< [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md) >(ID : Integer) : [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md) — функция, осуществляющая поиск доставки в базе данных по ID и возвращающая найденное Delivery, если такое имеется; 
* GetID(Delivery: [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md)) : Integer — функция, возвращающая ID определенную доставку;
* SetDrTr([Driver](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Driver.md),[Transport](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Transport.md)):void – функция, позволяющая назначит водителя и т/с на доставку.
* GetDelivery (sorting : String, ASKorDESK : string, filterA : [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md), filterB : [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md), count : int, page : int) : List < [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md) > — функция, возвращающая список доставок с заданными параметрами.
 Параметры: 
-	sortintg: String– отвечает, по какому полю будет сортироваться список:
-	ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
-	filterA : [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md) – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
-	filterB : [Delivery](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Delivery.md) – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
-	count : Integer – отвечает, сколько элементов необходимо показать;
-	page: Integer – отвечает, с какой страницы начинать поиск элементов.

