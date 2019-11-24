## Описание интерфейса ISupplier
Интерфейс предназначен для работы с методами класса [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md)
## Реализация интерфейса
* Add (Supplier: [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md)) — функция, добавляющая поставщика в базу данных. Параметр «Supplier» — поставщик, которого необходимо добавить в БД;
* Del (Supplier: [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md)) — функция, удаляющая поставщика из программы. Параметр «Order» — поставщик, которого необходимо удалить из программы;
* Edit (Supplier: [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md)) — функция, редактирующая данные о поставщике. Параметр «Supplier» — поставщик, которого необходимо редактировать в БД;
* FindByID< [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md )>(ID : Integer) : [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md) — функция, осуществляющая поиск поставщика в базе данных по ID и возвращающая найденного Supplier, если такой имеется. 
* GetID(Supplier: Supplier) : Integer — функция, возвращающая ID определенного поставщика. 
* GetTopSup(Date1:DateTime,Date2:DateTime): List<Supplier> - функция, выводящая список топ поставщиков за оперделенный временной промежуток.
* GetProv(sorting : String, ASKorDESK : string, filterA : [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md), filterB : [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md), count : int, page : int) : List < [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md) > — функция, возвращающая список поставщиков с заданными параметрами.
 Параметры: 
-	sortintg: String– отвечает, по какому полю будет сортироваться список:
-	ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
-	filterA : [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md) – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
-	filterB : [Supplier](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Supplier.md) – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
-	count : int – отвечает, сколько элементов необходимо показать;
-	page: int – отвечает, с какой страницы начинать поиск элементов.
