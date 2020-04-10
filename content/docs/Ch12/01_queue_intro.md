# 佇列 Queue

> ![01_queue_is_not_queue.png](/img/Ch12/01_queue_is_not_queue.png)  

不知道各位有沒有排隊買東西的經驗呢？在沒有任何插隊、解壓縮及特權的狀況下，基本上就是先到先服務的，晚來的只好乖乖排隊等前面的離開。  
佇列跟排隊可說是一模一樣，皆具有「先進先出(First-In-First-Out)」的特性，而佇列的頭跟尾，分別就是排隊時的隊伍頭尾了。  
一般來說，佇列不存在長度限制，長度越長，所需的寫入跟讀取代價時間較高，不過佇列長度還是有可能取決於系統跟記憶體空間多寡。

(圖待補)  


## 新增/刪除資料
佇列在新增資料上有一定的規定，必須從後端(rear)進行新增，不能從其他位置新增資料(push)進去。  
佇列在刪除資料的時候也有規定，必須從前端(front)進行刪除，不能從其他位置刪除資料(pop)。  

(圖待補)  