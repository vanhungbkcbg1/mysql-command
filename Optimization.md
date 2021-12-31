#### Query Execution structure
![query execution](./images/query%20execution.png)
#### Clusted Index
leaf node is row data
(key and row data)
#### non-clusted index
leaf node is not row data, it will


#### Run query with no cache plan
SELECT SQL_NO_CACHE COUNT(*) FROM sakila.film_actor;

#### Get cost of the last query
SHOW STATUS LIKE 'last_query_cost';

#### output Explain
type: system,const,eq_ref,ref is good