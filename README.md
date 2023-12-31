# be-canonical [TODO]

Turn some expanded HTML into the smallest, optimized HTML representation so it can be rapidly cloned (via web components, for example)

```html
<my-ssr-web-component>
    <template shadowrootmode=open>
        <span itemprop>some dynamic data</span>
        <table>
            <thead>
            </thead>
            <tbody>
        </table>
        <be-canonical>
            <script type=application/json>
                {
                    "removeInner": [
                        "[itemprop]:not(itemscope)"
                        
                    ].
                    "removeOuter" : [
                        "tbody>tr:not([aria-index="0"])
                    ]
                }
            </script>
            <template>
            <template>
        </be-canonical>
    </template>
</my-ssr-web-component>
```