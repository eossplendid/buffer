
# buffer.c

  Tiny C string manipulation library.

## Installation

```
$ cpm install visionmedia/buffer.c
```

## API

```c
buffer_t *
buffer_new();

buffer_t *
buffer_new_with_size(size_t n);

buffer_t *
buffer_new_with_string(char *str);

buffer_t *
buffer_new_with_copy(char *str);

size_t
buffer_size(buffer_t *self);

size_t
buffer_length(buffer_t *self);

void
buffer_free(buffer_t *self);

int
buffer_prepend(buffer_t *self, char *str);

int
buffer_append(buffer_t *self, char *str);

int
buffer_equals(buffer_t *self, buffer_t *other);

buffer_t *
buffer_slice(buffer_t *self, size_t from, ssize_t to);

size_t
buffer_indexof(buffer_t *self, char *str);

void
buffer_fill(buffer_t *self, int c);
```

## License

  MIT
