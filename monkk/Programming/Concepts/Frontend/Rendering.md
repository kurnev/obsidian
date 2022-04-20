To render a page:

1. Browser parses all tags in HTML. When it touches `<script>` it immediateally stops and sync waits for its downloading and completion.
2. Build DOM
3. Build CSSSOM
4. Build render-tree
5. Reflow
6. Repaint

Reflow always triggers repaint