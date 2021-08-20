# NLP_Training5
---
### To Training tensorflow model
```
trainModel()
 ```
 ---
 ### To Predict the string
 ```
  #load test Data
  testList = readData("translation2019zh_valid.json")
  txt_list = exportDataWithFormat(testList)
  writeTotxt(txt_list,"engChineseTest.txt")
  test_input,test_target,_,_ =readFormatTextToList("engChineseTest.txt")

  #predict
  predictTxt(test_input[:100],test_target[:100])
 ```
