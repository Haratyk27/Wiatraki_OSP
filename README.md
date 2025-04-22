# Wiatraki_OSP
 Projekt badanie wibracji wiatraków komputerowych
Autorzy:
Kamil Haratyk
Jan Suchanek
Tadausz Dźwigoł
Opiekun projektu:
Roman Wyżgolik

Polecenie projektowe:
System analizy wibracji wentylatora komputerowego.
Należy zaopatrzyć się w wentylator dwa wentylatory komputerowe z możliwością
rejestracji prędkości obrotowej, przy czym w jednym dokonane zostanie uszkodzenie
jednej z łopatek, tak, żeby wymusić większy poziom wibracji.
Do dyspozycji będą akcelerometry półprzewodnikowe ADXL do pomiaru wibracji.
Wibracje jak i prędkość obrotowa wentylatora rejestrowana będzie przez kartę DAQ NI
USB-6003. Karta jest dostępna.
Rejestrowany sygnał wibracji prezentowany ma być on-line na wykresie oraz
przeprowadzana ma być analiza widma mocy (Power Spectrum) on-line.
Mile widziana możliwość regulacji prędkości obrotowej wentylatorów z poziomu aplikacji
LabVIEW.
Sygnał wibracji jaki i widmo mocy, po naciśnięciu przycisku RECORD, mają zostać
zapisane do pliku TDMS (format pliku to data.godina.minuta.sekunda.tdms) oraz do bazy
danych. Wybór bazy danych powinien być taki, aby umożliwić odczytywanie bazy z
wykorzystaniem platformy Grafana. UWAGA! Może się okazać, że nie da się zapisywać
bezpośrednio z LabVIEW do bazy danych (da się do SQL Server, SQLite) i trzeba będzie
zastosować rozwiązanie pośrednie (ODBC lub przez jakieś RestAPI).