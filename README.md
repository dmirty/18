split-dns

настраиваем split-dns
взять стенд https://github.com/erlong15/vagrant-bind

1)добавить еще один сервер client2

2)завести в зоне dns.lab 
имена
web1 - смотрит на клиент1
web2 смотрит на клиент2

https://github.com/dmirty/18/blob/master/dnslabweb1web2.JPG

3)зaвести еще одну зону newdns.lab

завести в ней запись
www - смотрит на обоих клиентов
https://github.com/dmirty/18/blob/master/newdns.lab.JPG




4)настроить split-dns

клиент1 - видит обе зоны newdns.lab и dns.lab, но в зоне dns.lab только web1
https://github.com/dmirty/18/blob/master/splitdns%20client1.JPG

клиент2 видит только dns.lab

https://github.com/dmirty/18/blob/master/splitdns%20web2.JPG


Также вот список зон
https://github.com/dmirty/18/blob/master/list%20of%20zones.JPG



