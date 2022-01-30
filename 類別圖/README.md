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
