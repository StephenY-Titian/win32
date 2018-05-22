---
Description: 'Occurs when the mouse wheel moves while the InkPicture control has focus.'
ms.assetid: 'f56a8af9-7618-4fa3-8dd5-aa81a7f817e4'
title: 'InkPicture.MouseWheel event'
---

# InkPicture.MouseWheel event

Occurs when the mouse wheel moves while the [InkPicture](inkpicture-control-reference.md) control has focus.

## Syntax


```C++
void MouseWheel(
  [in]������InkMouseButton ����������Button,
  [in]������InkShiftKeyModifierFlags Shift,
  [in]������long ��������������������Delta,
  [in]������long ��������������������x,
  [in]������long ��������������������y,
  [in, out]�VARIANT_BOOL ������������*Cancel
);
```



## Parameters

<dl> <dt>

*Button* \[in\]
</dt> <dd>

The button that was pressed.

</dd> <dt>

*Shift* \[in\]
</dt> <dd>

The state of the SHIFT key.

</dd> <dt>

*Delta* \[in\]
</dt> <dd>

The distance that the mouse wheel turned.

</dd> <dt>

*x* \[in\]
</dt> <dd>

The x-coordinate, in pixels, of the [**IInkCursor**](iinkcursor.md) object.

</dd> <dt>

*y* \[in\]
</dt> <dd>

The y-coordinate, in pixels, of the [**IInkCursor**](iinkcursor.md) object.

</dd> <dt>

*Cancel* \[in, out\]
</dt> <dd>

VARIANT\_TRUE to cancel the **MouseWheel** event for the parent control; otherwise, VARIANT\_FALSE.

</dd> </dl>

## Return value

This event does not return a value.

## Remarks

> [!Note]  
> The parameters *x* and *y* are in pixels, and not the HIMETRIC units that are associated with the ink space coordinate system. This is because this event replaces the related mouse event of an application that is not pen-aware, and that type of application refers only to pixels.

�

This event method is defined in the **\_IInkPictureEvents** interface. The **\_IInkPictureEvents** interface implements the [**IDispatch**](ebbff4bc-36b2-4861-9efa-ffa45e013eb5) interface with an identifier of DISPID\_IPEMouseWheel.

## Requirements



|                                     |                                                                                                                     |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�XP Tablet PC Edition \[desktop apps only\]<br/>                                                       |
| Minimum supported server<br/> | None supported<br/>                                                                                           |
| Header<br/>                   | <dl> <dt>Msinkaut.h (also requires Msinkaut\_i.c)</dt> </dl> |
| Library<br/>                  | <dl> <dt>InkObj.dll</dt> </dl>                               |



## See also

<dl> <dt>

[InkPicture](inkpicture-control-reference.md)
</dt> </dl>

�

�



