# Airflow-dags

To submit a DAG (Directed Acyclic Graph):

1. Open a terminal:
```
export AIRFLOW_HOME=/home/project/airflow
echo $AIRFLOW_HOME
cp my_first_dag.py $AIRFLOW_HOME/dags
```  
<br>

2. Verify that your DAG has been submitted:
```
airflow dags list
airflow dags list|grep "my-first-python-etl-dag"
```  
<br>

3. List out all the tasks in 'my-first-python-etl':
```
airflow tasks list my-first-python-etl-dag
```
<br>

4. If the DAG didn't get imported properly:
```
airflow dags list-import-errors
```
<br>
