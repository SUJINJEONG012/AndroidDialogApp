# AndroidDialogApp


# 코틀린 기반 안드로이드 앱 

---

<u></u>

- 퍼미션
- 다양한 다이얼로그 
  -  `토스트 메시지` 띄우기 
  -  `날짜` 또는 `시간` 입력받기
  -  `알림창` 띄우기
  - `커스텀 다이얼로그` 만들기
  
  
  
  
  ## 아이디 선언
  ```kotlin
  android:id="@+id/listBtn"
  ```
  
  
  
----




## 메인함수에 바인딩 선언 후, setOnClick리스너 함수로 기능구현
  
  ```kotlin
  binding.timeBtn.setOnClickListener {
           TimePickerDialog(this,object :TimePickerDialog.OnTimeSetListener{
               override fun onTimeSet(view: TimePicker?, hourOfDay: Int, minute: Int) {
                   Log.d("myLog", "선택한 시간은 :  ${hourOfDay}시 ${minute} 분 ")
               }
           },15,0,true).show()
        }
```




![20220922_155726](https://user-images.githubusercontent.com/56811978/191682530-77851a9b-6fee-42f2-bd86-2f0da69b8a54.jpg)

