# Truncate in tailwinds.

In Tailwind CSS, the truncate utility class can be used to truncate text that overflows its container. Here's how you can use it:

```plaintext
htmlCopy code<div class="truncate">
  This text will be truncated if it overflows its container.
</div>
```

This will truncate the text with an ellipsis (...) by default. You can also customize the truncation symbol by using the `truncate-{symbol}` variant:

```plaintext
htmlCopy code<div class="truncate truncate-clip">
  This text will be truncated with no symbol if it overflows its container.
</div>

<div class="truncate truncate-custom">
  This text will be truncated with a custom symbol if it overflows its container.
</div>
```

In the first example, the `truncate-clip` variant is used to truncate the text with no symbol. In the second example, a custom symbol is defined using the `truncate-custom` variant:

```plaintext
cssCopy code.truncate-custom {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  --tw-truncate-text: '***';
}
```

Here, the `--tw-truncate-text` custom property is used to define the truncation symbol. In this case, it's set to `***`. You can use any text or icon you like for the truncation symbol.