上傳檔案 :

scp -P 9091 <本地檔案絕對路徑> compchem@163.22.23.73:<遠端存放檔案絕對路徑>

e.g. :

scp -P 9091 /home/tenghongjun/results/y.file compchem@163.22.23.73:/home/compchem/thj

scp -P 9091

下載檔案 :

scp -P 9091 compchem@163.22.23.73:<遠端檔案絕對路徑> <本地存放檔案絕對路徑>

e.g. :

scp -P 9091 compchem@163.22.23.73:/home/compchem/thj/x.file /home/tenghongjun/results