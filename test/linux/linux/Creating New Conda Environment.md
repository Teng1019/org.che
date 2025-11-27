conda create 新環境

`conda create --name “環境名字” “預安裝package”`

`“預安裝package”通常是：1. anaconda(推薦，因爲已包括數據分析常用package） 2.python= x.x(x.x為版本號）`

`conda env lIst (check 所創環境名字）`

`conda install -c(選擇頻道） conda-forge (頻道） “package”`

`"package"實驗室裏通常為：cuda-toolkit(限Nvidia）openmm mdtraj mdanalysis packmol`

#會自適配當前環境的package 的版本
## mamba
推薦在base下載




