tw_zip_area
===========

#利用三碼郵遞區號反解行政區

請參閱 sample 
使用前需要載入 jquery 1.8以上版本
在#11 時利用 ajax 載入 $.ajax('zip_2_area.json', {dataType: "json"}) 取得 zip_2_area.json 地區資料，由於ajax 需要等待資料處理回傳所以會加上
chained = request.then
和
chained.done
來進行延遲處理


#getObjects
由於 zip_2_area.json 包含所有郵遞區號的節點
getObjects 這個 function 是用來查詢指定的 zip 在哪個 obj 節點中
