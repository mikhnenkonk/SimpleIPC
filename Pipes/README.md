Организуется двусторонний обмен данными по анонимному каналу между клиентом и сервером. 

Для этого дескрипторы чтения и записи анонимного канала используются как сервером, так и клиентом этого анонимного канала. 
После окончания чтения сервер записывает данные в канал, а клиент их читает. Для организации двустороннего обмена
данными по анонимному каналу сервер и клиенты канала синхронизируют доступ к этому каналу, чтобы исключить одновременный 
неконтролируемый доступ параллельных потоков к анонимному каналу. При отсутствии такой синхронизации возможно одновременное чтение
данных сервером и клиентом, т. к. они работают параллельно, и это вызовет неправильную работу программы и ее зависание.
