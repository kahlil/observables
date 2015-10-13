#### Mouse Drag Event
<pre><code class="javascript" data-trim>
let getElementDrags = (elmt) => {
    return dom.mousedown(elmt)
        .map((md) => dom.mousemove(document)
            .takeUntil(dom.mouseup(elmt))
        ).concatAll();
};

// Anwendung
getElementDrags(image)
    .forEach(moveImage)
</code></pre>
