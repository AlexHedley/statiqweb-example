# Docs

- [Libraries](LIBRARIES.md)

## Plugins

### Reading time

**Adding reading time estimates to blog posts from @ Jeremy Davis**

- https://blog.jermdavis.dev/posts/2023/reading-time-estimates-statiq

In your `appsettings.json` add a new _property_ and set the value:

`"ReadingSpeed": 100`

You can then override the `input/_header.cshtml` of your _theme_ and place it after the _tags_.

```html
<span>~@Model.GetString("ReadingTime") minutes</span>
```
