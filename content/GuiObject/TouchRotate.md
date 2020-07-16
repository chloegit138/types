The TouchRotate event fires when the player uses two fingers to make a pinch or pull gesture on the UI element using a touch-enabled device. Rotation occurs when the angle of the line between two fingers changes. This event fires in conjunction with [GuiObject.TouchPan](https://developer.roblox.com/api-reference/event/GuiObject/TouchPan). This event is useful for allowing the player to manipulate the rotation of UI elements on the screen.

This event fires with a table of [DataType.Vector2](https://developer.roblox.com/search#stq=Vector2) that describe the relative screen positions of the fingers involved in the gesture. In addition, it fires several times with multiple [Enum.UserInputState](https://developer.roblox.com/search#stq=UserInputState)s: Begin after a brief delay, Change when the player moves a finger during the gesture and finally once more with End.

Since this event requires at least two fingers, it is not possible to be simulated in Studio using the emulator and a mouse; you must have a real touch-enabled device (and also least two fingers, try asking a friend).

This event is part of a family of touch-related events. Other events like this one are [GuiObject.TouchTap](https://developer.roblox.com/api-reference/event/GuiObject/TouchTap), [GuiObject.TouchPinch](https://developer.roblox.com/api-reference/event/GuiObject/TouchPinch), [GuiObject.TouchPan](https://developer.roblox.com/api-reference/event/GuiObject/TouchPan), [GuiObject.TouchLongPress](https://developer.roblox.com/api-reference/event/GuiObject/TouchLongPress) and [Guiobject.TouchSwipe](https://developer.roblox.com/search#stq=TouchSwipe). In addition, `UserInputService` has a similarly named event that is not restricted to a specific UI element: [UserInputService.TouchRotate](https://developer.roblox.com/api-reference/event/UserInputService/TouchRotate).