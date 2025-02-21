# ansible-pos

#### Запускаем первоначальную настройку узла
##### *Эта команда запускатеся один раз для нового хоста*

```bash
# При выполнение команды потребуется ввести пароль от root
task pos kickstart lim= $host or $group
```

### Устанавливем необходмый софт

```bash
task pos inti=true lim= $host or $group
```

### Запускаем POS service

```bash
# Есть дополнительный параметр state=peresent or absent
task pos lim= $host or $group
```