# A. Install Java JDK
1. Go to https://www.oracle.com/in/java/technologies/downloads/#jdk21-windows**
2. Download JDK 21.01 ![17af54f48102ea589666a09b21943b30.png](_resources/17af54f48102ea589666a09b21943b30.png)
3. Install the JDK 
![1206bcd1c765fc080bad06198536092e.png](_resources/1206bcd1c765fc080bad06198536092e.png)
4. Check if JAVA is installed and working. Launch command prompt: `java --version`**
![54c5647f17e9425d8769e70f62adcc8c.png](_resources/54c5647f17e9425d8769e70f62adcc8c.png)
***
# B. Clone the github repository
Clone the repo:
```
git clone https://github.com/LazyRook01/PySpark-3.5.0_Setup.git
```
***
# C. Setup Environment Variables
![84c9dd4ecff4e1c652a32556a10981d7.png](_resources/84c9dd4ecff4e1c652a32556a10981d7.png)
![9930b79f1dd443d872483d91eacad391.png](_resources/9930b79f1dd443d872483d91eacad391.png)
![d3d2a4f1315b992d253c3a59d6767374.png](_resources/d3d2a4f1315b992d253c3a59d6767374.png)

**Note: variable value will be determined by the path where you cloned the repository.**

**Edit Path -> New**
![b1c0b79f0346091fada86630dbec8b05.png](_resources/b1c0b79f0346091fada86630dbec8b05.png)
***
# D. Jupyter Notebook
*The jupyter notebook is there on the repo as test_spark.ipynb*
**1. Install findspark**
`!python -m pip install findspark`
2. `import findspark
findspark.init()`
3. 
```python
import pyspark
from pyspark.sql import SparkSession
spark = SparkSession.builder.getOrCreate()
df = spark.sql("select 'spark' as hello ")
df.show()
```
**Output:**
![4db568acbf9996b857b1794810022397.png](_resources/4db568acbf9996b857b1794810022397.png)
