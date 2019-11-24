## Описание интерфейса IClient
Интерфейс предназначен для работы с методами класса [Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md)
## Реализация интерфейса
* Add (Client: [Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md)) — функция, добавляющая клиента в базу данных. Параметр «Client» — клиент, которого необходимо добавить в БД;
* Del (Client: [Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md)) — функция, удаляющая клиента из программы. Параметр «Client» — клиент, которого необходимо удалить из программы;
* Edit (Client: [Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md)) — функция, редактирующая данные о клиенте. Параметр «Client» — клиент, которого необходимо редактировать в БД;
* FindByID< Client >(ID : Integer) : Client — функция, осуществляющая поиск клиента в базе данных по ID и возвращающая найденного клиента, если такой имеется. 
* GetID(Client: [Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md)) : Integer — функция, возвращающая ID определенного клиента. 
* GetBestClients(Date1:DateTime,Date2:DateTime):List<[Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md)> - функция, возвращающая список топ клиентов в определенном временном промежутке.
* GetClientOrder(Date1:DateTime,Date2:DateTime):List<Order> - функция, позволяющая выводить список заказов клиента.
* GetClients(sorting : String, ASKorDESK : string, filterA : [Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md), filterB : [Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md), count : int, page : int) : List < Client > — функция, возвращающая список клиентов с заданными параметрами.
  Параметры: 
-	sortintg: String – отвечает, по какому полю будет сортироваться список:
-	ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
-	filterA : [Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md) – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
-	filterB : [Client](https://github.com/mrsmyc/itsaboutsmyc/blob/master/Client.md) – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
-	count : int – отвечает, сколько элементов необходимо показать;
-	page: int – отвечает, с какой страницы начинать поиск элементов.
