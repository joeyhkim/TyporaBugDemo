# TyporaBugDemo
Demonstrates the resize image bug for the following Typora bug report:

[https://github.com/typora/typora-issues/issues/1475](https://github.com/typora/typora-issues/issues/1475)

### Resize Images Using Width Attribute (not working)

According to the Typora documentation [here](https://support.typora.io/Resize-Image/), you can use the following html tag to resize images:

```html
<img src="url" width="200px" />
```

Such resizing is supported by GitHub and GitLab, but the images are not resizing properly in the Typora view. Changing the width attribute has no effect in Typora, but the changes reflect accurately on GitHub. 

For example, the following two images should be different sizes, but in the Typora view, they are exactly the same size:

<img src="/cat.jpg" width=40%>

<img src="/cat.jpg" width=10%>

### Image Resizing with the Style Attribute

Image size changes made using the style attribute do reflect accurately in the Typora view. Unfortunately, GitHub and GitlLab markdown do not support this attribute.