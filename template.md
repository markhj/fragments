# 📆 Add and subtract from date

The functions ``DATE_ADD`` and ``DATE_SUB`` let's you add/subtract from a given date.

````mysql
DATE_ADD(from, interval)
DATE_SUB(from, interval)
````

## ✏️ Examples
### Add 2 weeks to current date
````mysql
DATE_ADD(NOW(), INTERVAL 2 WEEK)
````

### Subtract 10 seconds from ``column_name``
````mysql
DATE_SUB(column_name, INTERVAL 10 SECOND)
````

### Subtract 48 hours from a specified date
````mysql
DATE_SUB("2024-02-09 15:00", INTERVAL 48 HOUR)
````

## Notes 📜
The interval must be written in singular form, even when in natural English, it
should have been plural. So ``2 WEEK``, _not_ ``2 WEEKS``.
