# RPGSHOP_Reloaded
這是一個以巴哈姆特插件RPGSHOP為參考重新製作的腳本  
另外新增了GUI編輯器功能，支援物品NBT自定義  
目前可用於交易的有 money,playerpoints,level,自定義物品  

## required plugins:
    Skript 2.3 ~ lastest
    skript-reflect
    skript-yaml
    vault
    PlayerPoints  (選)


## Server Version : 

spigot or parper 1.13.2 ~ 1.19.3

## Command & Permission
    /rsa editor - 打開GUI編輯器
    /rsa create [代號] - 創建一個商店
    /rsa setname [代號] [名稱] - 設定該商店的顯示名稱
    /rsa list [頁數] - 檢視所有商店 (一頁顯示20個)
    /rsa reload - 重新讀取腳本
    /rpgshop [player] [商店代號] - 開啟商店交易介面 (建議使用console運行)
  **permission: rsa.admin**

## API
  ```
  # Expressions
  # 查看玩家的point數量
  PlayerPoints_look(player)
  # 從字串中提取數字
  StringGetNumber(字串)
  
  #Conditions
  # 檢測某插件是否有讀取
  plugin_exists(字串)
  
  #Effect
  # 給予玩家point
  PlayerPoints_give(player,整數)
  # 設置玩家point
  PlayerPoints_set(player,整數)
  # 收取玩家point
  PlayerPoints_take(player,整數)
  ```


