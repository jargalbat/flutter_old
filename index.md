---
layout: default
---

# Flutter animation
Flutter-ийн анимэйшн систем нь `Animation` обьектүүд дээр тулгуурладаг.
#### Animation&lt;double&gt;
Animation обьект нь onscreen буюу дэлгэцтэй холбоо хамааралгүйгээр, тусдаа бие даан ажилладаг. Тодруулбал animation обьект болон render хийх, build функцүүдийн хооронд огт хамаарал байхгүй. Animation абстракт класс нь одоогийн утга, дууссан, хаагдсан төлөвийг л ойлгодог. Хамгийн түгээмэл ашиглагддаг анимэйшны нэг төрөл нь `Animation<double>`. Animation обьект нь тодорхой хугацаанд 2 утгын хооронд дараалсан тоонуудыг үүсгэнэ. Animation обьектийн гаралт нь шугаман, муруй, тодорхой алхамтай функц, мөн түүнчлэн хөгжүүлэгчийн өөрөө тодорхойлсон ямар нэг дүрслэл байж болно. Animation обьектийг хэрхэн удирдаж байгаагаас хамаарч хөрвөх, чиглэл нь өөрчлөгдөх зэрэг үйлдэл хийгдэнэ. Animation обьект өөрийн гэсэн state-тэй байх бөгөөд `.value`-д яг одоогийн state хадгалагдана.
Animation нь double-аас гадна өнгө `Animation<Color>`, хэмжээ `Animation<Size>` төрөлтэй байж болно.
#### Curved­Animation
Муруйн дагуу өөрчлөгдөх анимэйшний алхмуудыг CurvedAnimation-ээр тодорхойлно. 
```dart
animation = CurvedAnimation(parent: controller, curve: Curves.easeIn);
```
Curve class-ийг ашиглан дурын муруйг үүсгэж болно.
```dart
import 'dart:math';

class ShakeCurve extends Curve {
  @override
  double transform(double t) => sin(t * pi * 2);
}
```
CurvedAnimation, AnimationController нь хоёулаа `Animation<double>` төрөлтэй.
#### AnimationController









Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
