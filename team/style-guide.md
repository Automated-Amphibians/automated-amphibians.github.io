---
layout: content
---

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5

Paragraphs of text.

[A link](http://google.com)

A simple image.
![alt text](android-chrome-192x192.png)

A linked image.
[![alt text](android-chrome-192x192.png)](http://google.com)


##### Un-numbered lists

* List 1
* List 2
* List 3
* List 4

##### Numbered lists

1. Numbered List 1
    1. Numbered List 1
    1. Numbered List 1
1. Numbered List 2
1. Numbered List 3
1. Numbered List 4

##### Quotes

> Quoted section, lots of text
> Stays on the same line.

> You can have more.
    
##### Code:

    public void function() {

    }

or

```java
public void function() {

}
```


#### Tables:
Note: Important to note that tags must be closed or the page will fall apart.
<table>
 <tr>
 <th> Column 1</th>
 <th> Column 2</th>
 <th> Column 3</th>
 </tr>
 <tr>
 <td> Row 1, Col 1 </td>
 <td> Row 1, Col 2</td>
 <td> Row 1, Col 3</td>
 </tr>
 <tr>
 <td> Row 1, Col 1</td>
 <td> Row 1, Col 2</td>
 <td> Row 1, Col 3</td>
 </tr>
</table> 

[//]: Reminder of how to use comments.

:smile:

{% for file in site.static_files %}
  {% if file.extname == ".jpg" -%}
     * [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
  {%- endif %}
{% endfor %}

?
