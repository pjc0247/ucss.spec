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

Conditions
----
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
