# 测试阶段

## 一、数据集收集&处理

### 1. 收集数据

使用如下命令来收集数据：

```bash
conda activate simlingo
./start.sh
python data_collection.py
```

```text
备注1：start.sh 中需要修改的内容如下：
export CARLA_ROOT=/home/kemove/ll/simlingo/carla0915     # carla 0.9.15版本的根目录
export WORK_DIR=/home/kemove/ll/simlingo_liulei          # 当前项目的根目录

备注2：data_collection.py 中需要修改的内容如下：
    code_root   = r"/home/kemove/ll/simlingo_liulei"                  # 修改位置1：项目根目录
    carla_root  = "/home/kemove/ll/simlingo/carla0915"                # 修改位置2：carla根目录
    root_folder = r"/home/kemove/ll/database/"                        # 修改位置3：数据集存放的根目录

    route_folder = f"/home/kemove/ll/data/simlingo"                   # 修改位置4：收集路线文件(.xml)存放的位置
    
        routes = ["/home/kemove/ll/A论文/露天矿山VLA/data/simlingo/mine_train/1tu3_wandao.xml"]  # 修改位置5：收集路线文件(.xml)存放的位置
```