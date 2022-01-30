# 類別圖
可以顯示類別成員變數、函式、繼承、參考關係。  
描繪類別間描述原始程式等級的依賴關係。

### 基礎知識
1.類別  
![image](/類別圖/assets/1.jpg)

```csharp
public class Dialer
{
}
```
![image](/類別圖/assets/2.jpg)

```csharp
public class Dialer
{
  private ArrayList _digits;
  private int _nDigits;
  public void Digit(int n);
  protected bool RecordDigit(int n);
}
```
-表示private、#表示protected、+表示public

2.關聯  
![image](/類別圖/assets/3.jpg)
```csharp
public class Phone
{
  private Button _buttons[15];
}
```
如果要表示一對多的話:
![image](/類別圖/assets/4.jpg)
```csharp
public class Phonebook
{
  private ArrayList _pnos;
}
```
