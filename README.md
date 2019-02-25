# README

Start the application with Scout DevTrace enabled

```
SCOUT_DEV_TRACE=true rails s
```

The page will crash as soon as the `Post` route is rendered, with a stack level too deep error.

There are two ways to fix this:

1) Remove the `meta-tags` gem
2) Modify the `index.html` template for posts to not render as a collection