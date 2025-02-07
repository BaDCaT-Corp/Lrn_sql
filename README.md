# Lrn_sql
### Изучение команд SQL и примеры

Запрос находит самый населённый город в каждом штате:
SELECT 
    name
    ,(SELECT max(pop) FROM cities WHERE cities.state = states.name)
 FROM states;