ucss.spec
====
UnityCSS<br>
__[implementation](https://github.com/pjc0247/uss/tree/master/src/Assets/USS/Script/Parser)__ 

Basic Structure
----
```css
cond1 cond2 ... {
  property-key: property-value;
  /* ... */
}
```

Selectors
----
__ucss__ has 3 kinds of selector specifier.<br>
Each condition is similar to CSS'.
<br><br>
__Component (Same as `Element` in CSS)__
```css
RawImage { outline: #000000FF; }
```
__#ObjectName__
```css
#MyProfileImage { outline: #000000FF; }
```
__.ClassName__
```css
.outline { outline: #000000FF; }
```
You can use more than 2 conditions in one style. This will be evaluated as __'AND'__ operation.

Constants
----
```css
@primary: #0000FFFF;
@secondary: #000000FF;
@alert: #FF0000FF;

Text {
  color: @primary;
}
```

Bundle
----
```cs
@H1 {
  font-style: bold;
  font-size: 30;
}

Text {
  @h1;
}
```
