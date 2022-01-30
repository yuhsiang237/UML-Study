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

3.繼承  
![image](/類別圖/assets/5.jpg)
```csharp
public class Employee
{
  
}
public class SalariedEmployee : Employee
{

}
```
4.實作  
![image](/類別圖/assets/6.jpg)
```csharp
interface ButtonListener
{
  
}
public class ButtonDialerAdapter : ButtonListener
{

}
```
5.抽象類別  
![image](/類別圖/assets/7.jpg)
```csharp
public abstract class Shape
{
  private Point _points;
  public abstruct void Draw();
}
```
6.聚合  
![image](/類別圖/assets/8.jpg)
```csharp
public class Whole
{
  private Part _part;
}
```
聚合(aggregation)，意味整體/部分的關係，只是一種暗示。  

7.組合  
![image](/類別圖/assets/9.jpg)
```csharp
public class Owner
{
  private W _ward;
}
```
8.多重性  
![image](/類別圖/assets/10.jpg)
```csharp
public class BinaryTreeNode
{
  private BinaryTreeNode _leftNode;
  private BinaryTreeNode _rightNode;

}
```
