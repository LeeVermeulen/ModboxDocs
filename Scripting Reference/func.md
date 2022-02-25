---
title: "Func"
slug: "func"
hidden: false
createdAt: "2020-11-06T00:58:26.868Z"
updatedAt: "2021-06-18T13:58:42.884Z"
---
Functions avaiable in MBScript that return a value. Used in MBScript by: 'Func.Type.Name' 


[block:api-header]
{
  "title": "MB Variable"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Get Variable",
    "0-1": "MB Variable",
    "0-2": ""
  },
  "cols": 3,
  "rows": 1
}
[/block]

[block:api-header]
{
  "title": "Stored Entities Data"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "New(Entity, Bool)",
    "0-1": "Stored Entities Data",
    "0-2": "",
    "1-0": "New With Entities(Entity List, Bool)",
    "1-1": "Stored Entities Data",
    "1-2": ""
  },
  "cols": 3,
  "rows": 2
}
[/block]

[block:api-header]
{
  "title": "Play Time"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Time",
    "0-1": "Play Time",
    "0-2": "Time since start of the world's play mode"
  },
  "cols": 3,
  "rows": 1
}
[/block]

[block:api-header]
{
  "title": "Range"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "New(Number, Number)",
    "0-1": "Range",
    "0-2": "",
    "1-0": "Zero",
    "1-1": "Range",
    "1-2": "",
    "2-0": "Zero To One",
    "2-1": "Range",
    "2-2": ""
  },
  "cols": 3,
  "rows": 3
}
[/block]

[block:api-header]
{
  "title": "Color"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "White",
    "0-1": "Color",
    "0-2": "Solid White",
    "1-0": "Black",
    "1-1": "Color",
    "1-2": "Solid Black",
    "2-0": "Cyan",
    "2-1": "Color",
    "2-2": "",
    "3-0": "Clear",
    "3-1": "Color",
    "3-2": "",
    "4-0": "Grey",
    "4-1": "Color",
    "4-2": "",
    "5-0": "Gray",
    "5-1": "Color",
    "5-2": "",
    "6-0": "Magenta",
    "6-1": "Color",
    "6-2": "",
    "7-0": "Red",
    "7-1": "Color",
    "7-2": "",
    "8-0": "Yellow",
    "8-1": "Color",
    "8-2": "",
    "9-0": "Green",
    "9-1": "Color",
    "9-2": "",
    "10-0": "Blue",
    "10-1": "Color",
    "10-2": "",
    "11-0": "Lerp(Color, Color, Number)",
    "11-1": "Color",
    "11-2": "Linearly interpolates between colors a and b by t",
    "12-0": "Lerp Unclamped(Color, Color, Number)",
    "12-1": "Color",
    "12-2": "",
    "13-0": "New(Number, Number, Number, Number)",
    "13-1": "Color",
    "13-2": "",
    "14-0": "Random",
    "14-1": "Color",
    "14-2": "Generates a random color from HSV and alpha ranges"
  },
  "cols": 3,
  "rows": 15
}
[/block]

[block:api-header]
{
  "title": "Date Time"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Now",
    "0-1": "Date Time",
    "0-2": "",
    "1-0": "Today",
    "1-1": "Date Time",
    "1-2": "",
    "2-0": "Utc Now",
    "2-1": "Date Time",
    "2-2": "",
    "3-0": "New(Whole Number, Whole Number, Whole Number, Whole Number, Whole Number, Whole Number)",
    "3-1": "Date Time",
    "3-2": ""
  },
  "cols": 3,
  "rows": 4
}
[/block]

[block:api-header]
{
  "title": "Mathf"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "PI",
    "0-1": "Number",
    "0-2": "",
    "1-0": "Infinity",
    "1-1": "Number",
    "1-2": "",
    "2-0": "Negative Infinity",
    "2-1": "Number",
    "2-2": "",
    "3-0": "Deg2Rad",
    "3-1": "Number",
    "3-2": "Degrees-to-radians conversion constant",
    "4-0": "Rad2Deg",
    "4-1": "Number",
    "4-2": "Radians-to-degrees conversion constant",
    "5-0": "Abs",
    "5-1": "Number",
    "5-2": "Returns the absolute value",
    "6-0": "Acos",
    "6-1": "Number",
    "6-2": "Returns the arc-cosine - the angle in radians whose cosine is f",
    "7-0": "Asin",
    "7-1": "Number",
    "7-2": "Returns the arc-sine - the angle in radians whose sine is f.",
    "8-0": "Atan",
    "8-1": "Number",
    "8-2": "Returns the arc-tangent - the angle in radians whose tangent is f.",
    "9-0": "Atan2(Number, Number)",
    "9-1": "Number",
    "9-2": "Returns the angle in radians whose Tan is y/x.",
    "10-0": "Ceil",
    "10-1": "Number",
    "10-2": "Returns the smallest integer greater to or equal to f.",
    "11-0": "Clamp(Number, Number, Number)",
    "11-1": "Number",
    "11-2": "Clamps the given value between a range defined by the given minimum integer and maximum integer values. Returns the given value if it is within min and max.",
    "12-0": "Clamp01",
    "12-1": "Number",
    "12-2": "Clamps value between 0 and 1",
    "13-0": "Cos",
    "13-1": "Number",
    "13-2": "Returns the cosine of angle f",
    "14-0": "Delta Angle(Number, Number)",
    "14-1": "Number",
    "14-2": "Calculates the shortest difference between two given angles given in degrees",
    "15-0": "Exp",
    "15-1": "Number",
    "15-2": "Returns e raised to the specified power.",
    "16-0": "Floor",
    "16-1": "Number",
    "16-2": "Returns the largest integer smaller than or equal to f.",
    "17-0": "Lerp(Number, Number, Number)",
    "17-1": "Number",
    "17-2": "Linearly interpolates between a and b by t.",
    "18-0": "Lerp Angle(Number, Number, Number)",
    "18-1": "Number",
    "18-2": "Same as Lerp but makes sure the values interpolate correctly when they wrap around 360 degrees.",
    "19-0": "Log(Number, Number)",
    "19-1": "Number",
    "19-2": "Returns the natural (base e) logarithm of a specified number.",
    "20-0": "Log10",
    "20-1": "Number",
    "20-2": "Returns the base 10 logarithm of a specified number.",
    "21-0": "Max(Number, Number)",
    "21-1": "Number",
    "21-2": "Returns the largest value.",
    "22-0": "Min(Number, Number)",
    "22-1": "Number",
    "22-2": "Returns the smallest of two values.",
    "23-0": "Move Towards(Number, Number, Number)",
    "23-1": "Number",
    "23-2": "Moves a value current towards target.",
    "24-0": "Move Towards Angle(Number, Number, Number)",
    "24-1": "Number",
    "24-2": "Same as MoveTowards but makes sure the values interpolate correctly when they wrap around 360 degrees.",
    "25-0": "Pow(Number, Number)",
    "25-1": "Number",
    "25-2": "Returns f raised to power p.",
    "26-0": "Sign",
    "26-1": "Number",
    "26-2": "Returns the sign of f.",
    "27-0": "Sin",
    "27-1": "Number",
    "27-2": "Returns the sine of angle f.",
    "28-0": "Smooth Step(Number, Number, Number)",
    "28-1": "Number",
    "28-2": "Interpolates between min and max with smoothing at the limits.",
    "29-0": "Sqrt",
    "29-1": "Number",
    "29-2": "Returns square root of f.",
    "30-0": "Tan",
    "30-1": "Number",
    "30-2": "Returns the tangent of angle f in radians.",
    "31-0": "Log Base(Number, Number)",
    "31-1": "Number",
    "31-2": "Returns the logarithm of a specified number in a specified base.",
    "32-0": "Round",
    "32-1": "Number",
    "32-2": "",
    "33-0": "Round To(Whole Number)",
    "33-1": "Number",
    "33-2": ""
  },
  "cols": 3,
  "rows": 34
}
[/block]

[block:api-header]
{
  "title": "Random"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Value",
    "0-1": "Number",
    "0-2": "Returns a random number between 0.0 [inclusive] and 1.0 [inclusive]",
    "1-0": "Range(Number, Number)",
    "1-1": "Number",
    "1-2": "Return a random float number between min [inclusive] and max [inclusive]",
    "2-0": "On Unit Sphere",
    "2-1": "Vector3",
    "2-2": "Returns a random point on the surface of a sphere with radius 1",
    "3-0": "Inside Unit Circle",
    "3-1": "Vector2",
    "3-2": "Returns a random point inside a circle with radius 1",
    "4-0": "Inside Unit Sphere",
    "4-1": "Vector3",
    "4-2": "Returns a random point inside a sphere with radius 1"
  },
  "cols": 3,
  "rows": 5
}
[/block]

[block:api-header]
{
  "title": "Time"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Realtime Since Startup",
    "0-1": "Number",
    "0-2": "Real time in Seconds since Modbox started",
    "1-0": "Delta Time",
    "1-1": "Number",
    "1-2": "Time in Seconds since last frame",
    "2-0": "Fixed Delta Time",
    "2-1": "Number",
    "2-2": "Interval which physics updates",
    "3-0": "World Play Time",
    "3-1": "Number",
    "3-2": "Time since play mode began in World"
  },
  "cols": 3,
  "rows": 4
}
[/block]

[block:api-header]
{
  "title": "Text"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "New Line",
    "0-1": "Text",
    "0-2": ""
  },
  "cols": 3,
  "rows": 1
}
[/block]

[block:api-header]
{
  "title": "Transform Part"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Can See Other Transform(Transform Part)",
    "0-1": "Bool",
    "0-2": "",
    "1-0": "Angle To Other Transform(Transform Part)",
    "1-1": "Number",
    "1-2": ""
  },
  "cols": 3,
  "rows": 2
}
[/block]

[block:api-header]
{
  "title": "MB Type"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Get MB Type",
    "0-1": "MB Type",
    "0-2": "",
    "1-0": "As Type(MB Type)",
    "1-1": "Object of any Type",
    "1-2": "Returns as the given Type (if it is the type / can convert to type)",
    "2-0": "Is Type(MB Type)",
    "2-1": "Bool",
    "2-2": ""
  },
  "cols": 3,
  "rows": 3
}
[/block]

[block:api-header]
{
  "title": "Vector2"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Zero",
    "0-1": "Vector2",
    "0-2": "",
    "1-0": "One",
    "1-1": "Vector2",
    "1-2": "",
    "2-0": "Up",
    "2-1": "Vector2",
    "2-2": "",
    "3-0": "Down",
    "3-1": "Vector2",
    "3-2": "",
    "4-0": "Right",
    "4-1": "Vector2",
    "4-2": "",
    "5-0": "Left",
    "5-1": "Vector2",
    "5-2": "",
    "6-0": "Distance(Vector2)",
    "6-1": "Number",
    "6-2": "Returns the distance between a and b.",
    "7-0": "Dot(Vector2)",
    "7-1": "Number",
    "7-2": "Dot Product of two vectors.",
    "8-0": "Lerp(Vector2, Number)",
    "8-1": "Vector2",
    "8-2": "Linearly interpolates between vectors a and b by t.",
    "9-0": "Move Towards(Vector2, Number)",
    "9-1": "Vector2",
    "9-2": "Moves a point current towards target.",
    "10-0": "Angle(Vector2)",
    "10-1": "Number",
    "10-2": "Returns the unsigned angle in degrees between from and to.",
    "11-0": "Signed Angle(Vector2)",
    "11-1": "Number",
    "11-2": "Returns the signed angle in degrees between from and to.",
    "12-0": "Scale(Vector2)",
    "12-1": "Vector2",
    "12-2": "Multiplies two vectors component-wise.",
    "13-0": "Reflect(Vector2, Vector2)",
    "13-1": "Vector2",
    "13-2": "Reflects a vector off the vector defined by a normal.",
    "14-0": "New(Number, Number)",
    "14-1": "Vector2",
    "14-2": ""
  },
  "cols": 3,
  "rows": 15
}
[/block]

[block:api-header]
{
  "title": "Vector3"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Zero",
    "0-1": "Vector3",
    "0-2": "",
    "1-0": "One",
    "1-1": "Vector3",
    "1-2": "",
    "2-0": "Up",
    "2-1": "Vector3",
    "2-2": "",
    "3-0": "Down",
    "3-1": "Vector3",
    "3-2": "",
    "4-0": "Right",
    "4-1": "Vector3",
    "4-2": "",
    "5-0": "Left",
    "5-1": "Vector3",
    "5-2": "",
    "6-0": "Forward",
    "6-1": "Vector3",
    "6-2": "",
    "7-0": "Back",
    "7-1": "Vector3",
    "7-2": "",
    "8-0": "Distance(Vector3)",
    "8-1": "Number",
    "8-2": "Returns the distance between a and b.",
    "9-0": "Dot(Vector3)",
    "9-1": "Number",
    "9-2": "Dot Product of two vectors.",
    "10-0": "Lerp(Vector3, Number)",
    "10-1": "Vector3",
    "10-2": "Linearly interpolates between vectors a and b by t.",
    "11-0": "Move Towards(Vector3, Number)",
    "11-1": "Vector3",
    "11-2": "Moves a point current towards target.",
    "12-0": "Angle(Vector3)",
    "12-1": "Number",
    "12-2": "Returns the unsigned angle in degrees between from and to.",
    "13-0": "Signed Angle(Vector3, Vector3)",
    "13-1": "Number",
    "13-2": "Returns the signed angle in degrees between from and to.",
    "14-0": "Rotate Towards(Vector3, Number, Number)",
    "14-1": "Vector3",
    "14-2": "Rotates a vector current towards target.",
    "15-0": "Scale(Vector3)",
    "15-1": "Vector3",
    "15-2": "Multiplies two vectors component-wise.",
    "16-0": "Reflect(Vector3, Vector3)",
    "16-1": "Vector3",
    "16-2": "Reflects a vector off the vector defined by a normal.",
    "17-0": "Project(Vector3, Vector3)",
    "17-1": "Vector3",
    "17-2": "Projects a vector onto another vector.",
    "18-0": "Project On Plane(Vector3, Vector3)",
    "18-1": "Vector3",
    "18-2": "Projects a vector onto a plane defined by a normal orthogonal to the plane.",
    "19-0": "Slerp(Vector3, Vector3, Number)",
    "19-1": "Vector3",
    "19-2": "Spherically interpolates between two vectors.",
    "20-0": "New(Number, Number, Number)",
    "20-1": "Vector3",
    "20-2": ""
  },
  "cols": 3,
  "rows": 21
}
[/block]