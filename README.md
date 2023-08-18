# weavejs
Webstandards-inspired Model-View-ViewModel library

```html
<x-counter>A Counter</x-counter>

<!-- x-counter.html -->
<template>
    <h1><slot></slot></h1>
    <button onclick.bind="increment()">+ ${count}</button>
    <script type="module">

        class Component {
            count = 0;

            increment() {
                this.count += 1;
            }
        }

    </script>
</template>
```