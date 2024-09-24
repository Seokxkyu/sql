## 문제 1
### 우리 플랫폼에 정착한 판매자 1

```sql
SELECT 
    seller_id, 
    COUNT(DISTINCT order_id) AS orders
FROM 
    olist_order_items_dataset
GROUP BY 
    seller_id
HAVING 
    orders >= 100
ORDER BY 
    orders DESC;
```
![image](https://github.com/user-attachments/assets/eb800d3c-23f2-4cd4-b90e-8c883e676072)


## 문제 2
### 몇 분이서 오셨어요?

```sql
SELECT *
FROM tips
WHERE MOD(size, 2) = 1;
```
![image](https://github.com/user-attachments/assets/d553c7e5-722c-4b15-8691-fa11668808ee)


## 문제 3
### 최고의 근무일을 찾아라

```sql
SELECT 
    day, 
    ROUND(SUM(tip), 3) AS tip_daily
FROM 
    tips
GROUP BY 
    day
ORDER BY 
    tip_daily DESC
LIMIT 1;
```
![image](https://github.com/user-attachments/assets/bf177402-300d-4fdf-84bd-454ba8e9f532)
