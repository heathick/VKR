# VKR

### Создание смарт-контракта

Теперь можно использовать следующий код javascript для развертывания смарт-контракта. 

`node deploy.js`

Когда транзакция упакована в блок, можно получить адрес контракта (например, 0x917.....da3) и значение abi. Необходимо изменить значение адреса контракта в *instance.js*. Более того, в *instance.js* также необходимо закрыть значение abi.  

### Генерирование открытого/закрытого ключа для клиента

Для каждого клиентского узла можно запустить команду *generateKey.js* для генерации пары открытый/закрытый ключ. Этот открытый ключ, связанный с адресом клиента, будет опубликован в блокчейне. Например, можно сгенерировать пару ключей для узла 1 следующим образом. 
`node generateKey.js`

### Request service

На этом этапе клиент записывает в смарт-контракт адрес поставщика услуг и данные идентификатора услуги. Этот идентификатор является уникальным в данной системе. Можно запустить JavaScript-код *requestService.js* для имитации процесса запроса.

`node requestService.js`

### Promise service

Фаза promise_service записывает хэш-значение в смарт-контракт. Можно запустить *promiseService.js* для имитации процесса обещания.

`node promiseService.js`

### Confirm service

На этапе confirm_service предлагаемая схема проверяет, совпадают ли два хэш-значения.  Один раз можно запустить *confirmService.js* для имитации процесса подтверждения.

`node confirmService.js`

### Send key

Для фазы send_key предложенная схема требует записи ключа расшифровки в смарт-контракте. Однако его размер меньше. Один раз можно запустить sendKey.js, чтобы смоделировать процесс отправки ключа.

`node sendKey.js`
