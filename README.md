# Belajar SQL

> Ini adalah artikel belajar SQL dari mulai Syntax dan sebagainnya.

## Selecting Data

- Gunakan syntax `SELECT * FROM (database);` untuk mengambil seluruh column.
```sql
SELECT * FROM student;
```

- Gunakan syntax `SELECT (column1), (column2) FROM (database);` untuk mengambil column1 dan column1 saja.
Digunakan untuk mengambil kolom tertentu saja
```sql
SELECT nama, usia FROM student;
```

- Gunakan syntax `SELECT DISTINCT (column1) FROM (database);` untuk mengambil ringkasan data.
```sql
SELECT DISTINCT kelas FROM student;
```

## Ordering Data

- Gunakan syntax `SELECT * FROM (database) ORDER BY (column1);` untuk mengambil seluruh data column dengan ASCENDING atau berurutan dari huruf atau angka awal (A/0).
```sql
SELECT * FROM student ORDER BY nama;
```

- Gunakan syntax `SELECT * FROM (database) ORDER BY (column1) DESC;` untuk mengambil seluruh data column dengan ASCENDING atau berurutan dari huruf atau angka akhir (z/9).
```sql
SELECT * FROM student ORDER BY nama DESC;
```

## Filtering Data

- Gunakan syntax `SELECT * FROM (database) WHERE (column1) = 'value';` digunakan untuk mengambil data sesuai dengan `value` yang diberikan.
```sql
SELECT * FROM student WHERE class = "Management Informatics";
```

## Comparisons Data

- Gunakan syntax `SELECT * FROM (database) WHERE (column1) < number;` digunakan untuk mengambil data sesuai dengan `value` yang diberikan.
```sql
SELECT * FROM student WHERE age = 14;
```

- Gunakan syntax `SELECT * FROM (database) WHERE (column1) <> number;` digunakan untuk mengambil data yang tidak sesuai dengan `value` yang diberikan.
```sql
SELECT * FROM student WHERE age <> 17;
```

- Gunakan syntax `SELECT * FROM (database) WHERE (column1) < number;` digunakan untuk mengambil data yang lebih kecil dengan `value` yang diberikan.
```sql
SELECT * FROM student WHERE age < 17;
```

```sql
SELECT * FROM student WHERE age <= 17;
```

- Gunakan syntax `SELECT * FROM (database) WHERE (column1) < number;` digunakan untuk mengambil data yang lebih besar dengan `value` yang diberikan.
```sql
SELECT * FROM student WHERE age > 17;
```

```sql
SELECT * FROM student WHERE age >= 17;
```

## Filtering With Ranges

- Gunakan syntax `SELECT * FROM (database) WHERE (column1) BETWEEN 6 AND 10;` digunakan untuk mengambil data diantara `value` yang diberikan.
```sql
SELECT * FROM books WHERE price BETWEEEN 1000 AND 5000;
```

