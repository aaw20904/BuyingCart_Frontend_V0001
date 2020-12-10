This is a client`s part of online "only one page" food shop (bread,milk,potato e.t.c.).I tried to write this code in according to the SOLID principles.The application has a main part- UseCase Interactor.
This part interacts with a Modell, a Presenter,a stock interface (get info about item (like a name,a price..).The Use Case Interactor processing events through an interface "regEventsTranslator"
(events are simple strings in form "<ID>#<EVENT>").A Presenter has  interfaces to Use Case Interactor - "regEventsTranslator() regCallbackStockQuery() PresenterInput().
The Presenter interacts with DOM through several interfaces: objects "StringBinder, CheckOutHandler, StringUpdater, ProdString, CollectionStat CheckOutHandler".
These interfaces interacts directly with the DOM - there are not ANY libraries like JQuery.Here are several caps - because it is not no remote server.
