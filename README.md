# SQL-project
## Select all from cleaned_file
```sql
SELECT * FROM cleaned_file;
```
<img width="877" alt="Screenshot 1446-08-12 at 11 44 02 AM" src="https://github.com/user-attachments/assets/c2596d15-5bfd-416a-996b-c2c251e08241" />

## Count total records
```sql
SELECT COUNT(*) FROM cleaned_file;
```
<img width="255" alt="Screenshot 1446-08-12 at 11 45 11 AM" src="https://github.com/user-attachments/assets/628bf94a-10b7-48f3-bdba-dd6a6523c35c" />

## Retrieve all unique genres
```sql
SELECT DISTINCT genre FROM cleaned_file;
```
<img width="295" alt="Screenshot 1446-08-12 at 11 46 19 AM" src="https://github.com/user-attachments/assets/82623f59-c978-4e08-a477-88d14559493d" />

## Find the top 5 highest-rated places
```sql
SELECT name, rating FROM cleaned_file ORDER BY rating DESC LIMIT 5;
```
<img width="350" alt="Screenshot 1446-08-12 at 11 47 00 AM" src="https://github.com/user-attachments/assets/4f571564-1c52-49f8-aff2-d08fbd8d1154" />

## Count how many places have a rating of 4 or higher
```sql
SELECT COUNT(*) FROM cleaned_file WHERE rating >= 4;
```
<img width="255" alt="Screenshot 1446-08-12 at 11 47 53 AM" src="https://github.com/user-attachments/assets/53c2eb8d-815c-4ff7-978e-7d3c65df121c" />

## Find locations with missing best_comment
```sql
SELECT name, location FROM cleaned_file WHERE best_comment IS NULL;
```
<img width="341" alt="Screenshot 1446-08-12 at 11 48 43 AM" src="https://github.com/user-attachments/assets/12e3dc3a-71d2-4358-8579-a2ff66578dfc" />

## select all with review_count > 9900;
```sql
select  * from cleaned_file where review_count > 9900;
```
<img width="867" alt="Screenshot 1446-08-12 at 11 49 42 AM" src="https://github.com/user-attachments/assets/a7b0d86f-7a93-438f-9e43-6afe04755ed1" />

## Find the number of locations per genre
```sql
SELECT genre, COUNT(*) AS total FROM cleaned_file GROUP BY genre;
```
<img width="328" alt="Screenshot 1446-08-12 at 11 51 02 AM" src="https://github.com/user-attachments/assets/6c729c59-dcd6-4ebf-a1cb-c747b1f40e2e" />

## Find the average rating for movie theaters
```sql
SELECT AVG(rating) FROM cleaned_file WHERE genre = ' Movie theater';
```
<img width="279" alt="Screenshot 1446-08-12 at 11 52 13 AM" src="https://github.com/user-attachments/assets/c1d63501-48fc-4238-93d2-be0899572b69" />

## Find all places located in Saudi Arabia
```sql
SELECT name, location FROM cleaned_file WHERE location LIKE '%Saudi Arabia%';
```
<img width="500" alt="Screenshot 1446-08-12 at 11 53 13 AM" src="https://github.com/user-attachments/assets/5419c483-73fb-40ae-81f2-95024e4cd655" />

## Find all locations with a rating of 0
```sql
SELECT name, location FROM cleaned_file WHERE rating = 0;
```
<img width="475" alt="Screenshot 1446-08-12 at 11 53 57 AM" src="https://github.com/user-attachments/assets/21275c52-da3d-456d-80b1-1aa87189f546" />



