---
## 数据集

### SPATIAL 和 SPATIAL
* **名称**：3D 空间网络
* **文件**：`3D_spatial_network.txt` 和 `2D_spatial_network.txt`
* **来源**：[https://archive.ics.uci.edu/ml/datasets/3D+Road+Network+(North+Jutland,+Denmark](https://archive.ics.uci.edu/ml/datasets/3D+Road+Network+(North+Jutland,+Denmark))
* **预处理**：
    * **SPATIAL3D**：移除了 OSM_ID 属性（第一列）。
    * **SPATIAL**：移除了 OSM_ID 属性（第一列）和海拔（最后一列）。

### NGSIM
* **名称**：下一代模拟（NGSIM）车辆轨迹和支持数据
* **文件**：`Next_Generation_Simulation_(NGSIM).txt`
* **来源**：[https://www.opendatanetwork.com/dataset/data.transportation.gov/8ect-6jqj](https://www.opendatanetwork.com/dataset/data.transportation.gov/8ect-6jqj)
* **预处理**：
    * 地理位置数据点从 Local_X 和 Local_Y 属性中提取。

### PORTO
* **名称**：出租车服务轨迹 - 预测挑战，ECML PKDD 2015 数据集
* **文件**：`Porto_Taxi_Service_Trajectory.txt`
* **来源**：[https://archive.ics.uci.edu/ml/datasets/Taxi+Service+Trajectory+-+Prediction+Challenge,+ECML+PKDD+2015](https://archive.ics.uci.edu/ml/datasets/Taxi+Service+Trajectory+-+Prediction+Challenge,+ECML+PKDD+2015)
* **预处理**：
    * 除了 POLYLINE 属性，移除了所有其他属性。
    * 地理位置数据点从每行的数组中提取。

---
## 实验说明

在 HiPC 2021 的论文中，我们执行算法时会指定数据点的数量 $|D|$，这表示我们仅从数据集文件中读取前 $|D|$ 行数据。

---