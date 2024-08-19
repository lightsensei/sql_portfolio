#American baby names analysis

Project overview
     In this project, we will focusing on american baby names and analyse names in particular categories, find names that are timeless, and names that are trendy for a [articular period of time.

Data Overview
     This dataset contains 5 columns named index, name, sex, count and year respectively.

```sql
select name, year, sum(count) from american_baby_names
where year >= 1920
group by name, year
