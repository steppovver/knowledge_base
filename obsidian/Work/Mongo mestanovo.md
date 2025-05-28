## Первый этап
**Начало** -- 546874981
**Конец** -- 546877201

**Частота** -- 5470
**Аттенюация** -- 0

**Буфер анализа** -- 10мс

**Название баз**
1. mestanovo-16
2. mestanovo-18

## Второй этап
**Начало** -- 546878100
**Реальное начало по данным** -- 546878536
**Конец** -- 546879600
**Название баз**
1. mestanovo-16-2
2. mestanovo-18-2
## Баги
1. **DONE** Ловлю падение на
```
{ "user_info.timeUTC": 546875956 }

db.Data.deleteMany({ data_subtype: { $ne: "analysis" } })
db.Data.deleteMany({ "user_info.timeUTC": { $lt: 546875956 } })
db.Data.deleteMany({ "user_info.timeUTC": { $gt: 546875956 } })
```
2. **DONE** Найден багец
546878866 - время буфера анализа на котором в равках не находятся некоторые буфера анализа
```
db.Data.deleteMany({ data_subtype: { $ne: "analysis" } })
db.Data.deleteMany({ "user_info.timeUTC": { $lt: 546878866 } })
db.Data.deleteMany({ "user_info.timeUTC": { $gt: 546878866 } })
```
3. Покет если присылает пучтые буферы анализа, у них не правильное data_timestamp
4. **DONE** Перестает работать playback
**Время** с которого перестают обрабатываться буферы -- 546881405
Как будто нет ответа на рав икушки
```
12:38:29.756 default(Warning): QSocketNotifier: Socket notifiers cannot be enabled or disabled from another thread
```
## Полезные команды

Удалить лишние типы данных 
```
db.Data.deleteMany({ data_subtype: { $ne: "analysis" } })
```
Удалить данные меньше чем
```
db.Data.deleteMany({ "user_info.timeUTC": { $lt: 546881280 } })
```



